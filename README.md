# feedback-user
print("Enter feedbacks (type 'done' to finish):")

positive_words = ["good", "great", "awesome", "happy", "love", "excellent"]
negative_words = ["bad", "sad", "terrible", "hate", "poor", "worst"]

while True:
    feedback = input("> ")
    if feedback.lower() == "done":
        break

    text = feedback.lower()
    if any(word in text for word in positive_words):
        print("Sentiment: Positive 😊\n")
    elif any(word in text for word in negative_words):
        print("Sentiment: Negative 😞\n")
    else:
        print("Sentiment: Neutral 😐\n")
