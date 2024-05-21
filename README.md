# About WeatherToWear
WeatherToWear is a dynamic application that simplifies personal styling by suggesting outfits based on user inputs, such as personal style preferences, combined with real-time weather forecasting. By harnessing data from Rent the Runway and employing clustering algorithms, we aim to create a user-friendly interface that recommends the perfect outfit for any occasion, ensuring style suitability and weather appropriateness.

# Data Overview  
Our comprehensive dataset, sourced from the website Rent The Runway, features over 94,000 clothing items. We've meticulously categorized these items using the FashionCLIP model (Hugging Face) based on style, color, and weather suitability. Each entry includes the item's name and image URL, essential for the visual aspect of our application. This organized data allows users to easily filter and explore clothing options based on their specific needs.

# Advancements in ML  for Personalized Fashion Recommendations
In our project, the application of machine learning (ML) is pivotal in revolutionizing the way users interact with fashion technology. We utilize the FashionCLIP model, a variant of the CLIP (Contrastive Language–Image Pre-training) model trained specifically for fashion-related tasks. This model enables our system to understand complex, nuanced descriptions of clothing items and relate these to user inputs about style preferences and weather conditions.
Another significant aspect of our machine learning implementation is its adaptive nature. Our system is designed to learn continuously from user interactions. Every user feedback loop helps refine the model's accuracy, making the recommendations more personalized and relevant over time. This continuous learning is facilitated by the retraining protocols embedded in our ML setup, where new data from user interactions and ongoing trends are periodically integrated into the model.

# FashionCLIP Model Integration and Functionality
The integration of the FashionCLIP model into our backend allows us to categorize clothing items with high precision across multiple dimensions such as style, color, and weather appropriateness. For instance, when a user specifies a preference for a "bohemian" style of a "breathable" quality for the weather, the model can efficiently filter through thousands of items to suggest the most suitable outfits. This capability is supported by the model's training on a diverse set of fashion images and descriptive tags, enabling it to comprehend and predict user preferences with remarkable accuracy.

# Backend/Frontend Overview  
- Backend: Our backend consists of the classified dataset which enhances user experience by allowing precise outfit recommendations based on weather conditions and personal style.
Frontend: Developed using Streamlit and ngrok in Google Colab, our frontend comprises three main pages:
- Welcome: A minimalistic introduction featuring an image collage from Rent the Runway.
- Try it Out: Users are asked about their temperature preferences, then prompted by a button to gain access to their current location and weather conditions. Then, they select their stylistic preferences. All of these details interface with our backend to output an example image of a possible outfit.
- Our Data: Provides a deep dive into our dataset with statistics, previews, and visualizations to enhance user understanding and interaction.
