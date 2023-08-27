Markdown to HTML Converter
==========================

The Markdown to HTML Converter is a powerful command-line tool crafted in Rust, designed to seamlessly transform Markdown files into HTML. Built upon the robust `pulldown-cmark` crate, it ensures accurate parsing and rendering of Markdown content.

🌟 Features
-----------

*   **Swift Conversion**: Quickly turn your Markdown files into HTML.
*   **Intuitive CLI**: A user-friendly command-line interface with comprehensive argument parsing.
*   **Rich Markdown Support**: Handles a wide range of Markdown syntax including headings, paragraphs, lists, emphasis, links, images, and code blocks.
*   **Customization Options**: Enable specific Markdown features like tables and strikethrough.
*   **Flexible Output**: Directly save the generated HTML to your desired location or copy it directly to the clipboard.
*   **Theming**: Choose from multiple themes to style your HTML output.

🚀 Installation
---------------

1.  **Setup Rust Environment**: If Rust and Cargo aren't set up on your machine, get them from [Rust's official website](https://www.rust-lang.org/).
2.  **Clone the Repository**:
3.  
    ```console
    git clone https://github.com/arncv/MDtoHTM.git
    ```
    
4.  **Enter the Project Directory**:

    
    ```console
    cd markdown-to-html-converter
    ```
    
5.  **Compile the Project**:
    
    ```console
    cargo build --release
    ```
    

🛠 Usage
--------

Convert your Markdown to HTML with this simple command:


```console
cargo run --release -- -i <input-file> [-o <output-file>] [--theme <theme-name>]
```

*   `<input-file>`: Your Markdown file's path.
*   `<output-file>`: (Optional) Desired path for the HTML output. If not provided and the clipboard option is not used, an error will be displayed.
*   `--theme <theme-name>`: Optional theme (choices: default, dark, light).

**Example**: Convert `example.md` to HTML using the dark theme and save as `output.html`:

```console
cargo run --release -- -i example.md -o output.html --theme dark
```

Or, to copy the output directly to the clipboard:

```console
cargo run --release -- -i example.md --clipboard
```

🎨 Options
----------

*   **Theming**: Apply a theme to your HTML output.
    
    
    ```console
    cargo run --release -- -i <input-file> -o <output-file> --theme <theme-name>
    ```
    
*   **Tables**: Enable table formatting in your Markdown.
    
    
    ```console
    cargo run --release -- -i <input-file> -o <output-file> --tables
    ```
    
*   **Strikethrough**: Activate strikethrough formatting.
    
    
    ```console
    cargo run --release -- -i <input-file> -o <output-file> --strikethrough
    ```
    
*   **Clipboard Output**: Directly copy the generated HTML to the clipboard.
    
    
    ```console
    cargo run --release -- -i <input-file> --clipboard
    ```
    

🤝 Contributing
---------------

We value your contributions! Whether it's a feature request, bug fix, or a new idea, feel free to submit a pull request or open an issue. Let's make this tool even better, together!

📜 License
----------

This project is licensed under the [MIT License](LICENSE).