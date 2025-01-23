# Language Translation Tool 🌍✨

This is an interactive **Language Translation Tool** built using Python and the Google Translator API. It enables users to translate text between multiple languages seamlessly through a user-friendly interface.

## Features ✅
- **Dynamic Language Selection:** Choose both source and target languages from a dropdown menu.
- **Intuitive Input:** Enter text in a dedicated text area for translation.
- **Real-Time Output:** View translated text instantly in the output field.
- **Asynchronous Execution:** Ensures smooth and fast translations.

## Technologies Used 🛠️
- **Python**: For building the tool's functionality.
- **ipywidgets**: To create an interactive user interface in Jupyter Notebooks.
- **Googletrans**: For powerful and accurate translations.
- **asyncio**: To handle asynchronous operations efficiently.

## How to Use 🖥️
1. Clone the repository:
   ```bash
   git clone <https://github.com/Daniyal-DS/Code-Alpha-task-2>
   ```
2. Navigate to the project directory:
   ```bash
   cd language-translation-tool
   ```
3. Install the required libraries:
   ```bash
   pip install googletrans ipywidgets
   ```
4. Run the tool in a Jupyter Notebook or compatible environment.

## Code Snippet 📋
Here’s a glimpse of the main logic behind the tool:
```python
async def translator_function(from_lan, to_lan, t_text) -> str:
    Tt = ""
    try:
        async with Translator() as translator:
            translated_text = await translator.translate(t_text, src=from_lan, dest=to_lan)
            Tt = translated_text.text
    except:
        Tt = "Cannot translate"
    return f"{Tt}."
```

## Demo 🎥
Check out the demo video attached
## Contribution 🤝
Feel free to fork this repository and contribute to enhance the tool! Open a pull request with your suggestions and improvements.

## License 📜
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
