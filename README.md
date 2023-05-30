<!DOCTYPE html>
<html>
<head>
    <title>Fullscreen Iframe Example</title>
    <style>
        /* Define a CSS class for the fullscreen container */
        .fullscreen {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 9999;
        }

        /* Style the iframe to fill the fullscreen container */
        .fullscreen iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
    </style>
</head>
<body>
    <h1>Fullscreen Iframe Example</h1>
    
    <!-- Button to toggle fullscreen -->
    <button id="toggleFullscreen">Toggle Fullscreen</button>
    
    <!-- The iframe you want to display in fullscreen -->
    <iframe id="myIframe" src="[https://www.example.com](https://lookerstudio.google.com/embed/reporting/4ec967f1-6b6e-4a6d-9c5b-c3c78e06f433/page/KuRSD)"></iframe>

    <script>
        // Get references to the elements
        const toggleFullscreenBtn = document.getElementById('toggleFullscreen');
        const iframe = document.getElementById('myIframe');

        // Function to toggle fullscreen mode
        function toggleFullscreen() {
            // Toggle the "fullscreen" class on the iframe container
            iframe.parentNode.classList.toggle('fullscreen');
        }

        // Attach event listener to the toggle button
        toggleFullscreenBtn.addEventListener('click', toggleFullscreen);
    </script>
</body>
</html>
