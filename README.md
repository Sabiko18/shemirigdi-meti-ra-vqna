<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="./style/css/styles.css">
        <title>niakuna gtxov</title>
    </head> 
    <body>



       <style>











body  {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #F8C8DC;
}

/* Position the "No" button absolutely within body */
#noButton {
    position: absolute;
    margin-left: 150px;
    transition: 0.5s;
    /* Smooth movement */
}

#yesButton {
    position: absolute;
    margin-right: 150px;
    /* Smooth movement */
}

.header_text {
    font-family: 'Nunito';
    font-size: 50px;
    font-weight: bold;
    color: white;
    text-align: center;
    margin-top: 20px;
    margin-bottom: 0px;
}

.buttons {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
    margin-left: 20px;
    /* optional: adds some space between the buttons */
}

.btn {
    background-color: #FFB6C1;
    color: white;
    padding: 15px 32px;
    text-align: center;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
    border: none;
    border-radius: 12px;
    transition: background-color 0.3s ease;
}

.btn:hover {
    background-color: #FAF9F6;
}

.gif_container {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-left: 90px;
}
</style> <div class="container">
            <div >
                <h1 class = "header_text">Please can you forgive me very last time? </h1>
            </div>
            <div class="gif_container">
                <img src="https://media.giphy.com/media/LnKonfpQ44fNvuGLkA/giphy.gif" alt="Cute animated illustration">
            </div>
            <div class = "buttons">
                <button class="btn" id = "yesButton" onclick="nextPage()">Yes</button>
                <button class="btn" id="noButton" onmouseover="moveButton()">No</button>
                <script>
                    function nextPage() {
                        window.location.href = "yes.html";
                    }
                    
                    function moveButton() {
                        var x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth);
                        var y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight);
                        document.getElementById('noButton').style.left = `${x}px`;
                        document.getElementById('noButton').style.top = `${y}px`;
                    }
                </script> 
            </div>
        </div>
       
    </body> 
</html>
