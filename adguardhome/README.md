<!DOCTYPE html>
<html>
    <head>
        <title>AdGuardHome dockercompose.yaml README</title>
            <style>
            .code-container {
                position: relative;
                background-color: #2d2d2d;
                color: #ccc;
                padding: 1rem;
                border-radius: 8px;
                font-family: monospace;
                white-space: pre-wrap; /* Allows long lines to wrap */
                overflow: auto; /* Adds scrollbars if content is too large */
                max-height: 400px; /* Limits the height of the code block */
                margin-bottom: 1rem;
            }
            .copy-button {
                position: absolute;
                top: 10px;
                right: 10px;
                background-color: #555;
                color: white;
                border: none;
                padding: 8px 12px;
                border-radius: 4px;
                cursor: pointer;
                font-size: 14px;
                font-family: sans-serif;
                transition: background-color 0.2s;
            }
            .copy-button:hover {
                background-color: #777;
            }
            .copy-button:active {
                background-color: #444;
            }
            .copied-text {
                color: #4CAF50;
            }
    </style>
    </head>
    <body>
        <h1>AdGuardHome</h1>
        <p>Open the initial setup wizard and admin UI HTTP</p>
        <div class="code-container">
        <button class="copy-button" onclick="copyCode(this)">Copy</button>
    </div>
    <script>
        function copyCode(button) {
            // Select the code element inside the same parent as the button
            const codeBlock = button.parentNode.querySelector('code');
            // Create a temporary textarea to hold the code
            const tempTextArea = document.createElement('textarea');
            tempTextArea.value = codeBlock.textContent.trim();
            document.body.appendChild(tempTextArea);
            // Select the text and copy it
            tempTextArea.select();
            document.execCommand('copy');
            // Clean up the temporary textarea
            document.body.removeChild(tempTextArea);
            // Give the user visual feedback
            const originalText = button.textContent;
            button.textContent = 'Copied!';
            button.classList.add('copied-text');
            setTimeout(() => {
                button.textContent = originalText;
                button.classList.remove('copied-text');
            }, 2000);
        }
    </script> 
</html>