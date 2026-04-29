import requests

def emotion_detector(text_to_analyze):
    url = "https://api-inference.huggingface.co/models/j-hartmann/emotion-english-distilroberta-base"
    
    payload = {"inputs": text_to_analyze}
    headers = {"Content-Type": "application/json"}
    
    response = requests.post(url, json=payload, headers=headers)
    
    if response.status_code != 200:
        return {"error": "Unable to fetch emotion data"}
    
    data = response.json()[0]

    # Extract emotions
    emotions = {item['label']: item['score'] for item in data}

    # Find dominant emotion
    dominant_emotion = max(emotions, key=emotions.get)

    # Required formatted output
    return {
        "anger": emotions.get("anger", 0),
        "disgust": emotions.get("disgust", 0),
        "fear": emotions.get("fear", 0),
        "joy": emotions.get("joy", 0),
        "sadness": emotions.get("sadness", 0),
        "dominant_emotion": dominant_emotion
    }
