translations = {
    "greetings": {
        "Igbo": "Ndewo",
        "Hausa": "Sannu",
        "Yoruba": "Bawo",
        "Tiv": "M ngu",
        "Idoma": "Okwu"
    },
    "thank_you": {
        "Igbo": "Daalụ",
        "Hausa": "Na gode",
        "Yoruba": "E se",
        "Tiv": "Ior",
        "Idoma": "Okwu"
    },
    "how_are_you": {
        "Igbo": "Kedu?",
        "Hausa": "Lafiya?",

        "Idoma": "Okwu?"
    },
    "goodbye": {
        "Igbo": "Ka ọ dị",
        "Hausa": "Sai an jima",
        "Yoruba": "O dabọ",
        "Tiv": "A ka",
        "Idoma": "Okwu"
    },
    "yes": {
        "Igbo": "Ee",
        "Hausa": "I",
        "Yoruba": "Bẹẹni",
        "Tiv": "Ee",
        "Idoma": "E"
    }
}

# Function to translate back to English
def translate_to_english(translations):
    english_translations = {}
    for phrase, lang_dict in translations.items():
        english_translations[phrase] = {
            "Igbo": lang_dict["Igbo"],
            "Hausa": lang_dict["Hausa"],
            "Yoruba": lang_dict["Yoruba"],
            "Tiv": lang_dict["Tiv"],
            "Idoma": lang_dict["Idoma"]
        }
    return english_translations

# Print the original translations
print("Original Translations:")
for phrase, lang_dict in translations.items():
    print(f"{phrase}: {lang_dict}")

# Translate back to English
english_translations = translate_to_english(translations)

# Print the translated back to English
print("\nTranslated Back to English:")
for phrase, lang_dict in english_translations.items():
    print(f"{phrase}: {lang_dict}")
