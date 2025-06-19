# jsPopUp

## Description
The jsPopUp script is a simple JavaScript library that allows you to create and manage pop-up dialogs on your web pages. It provides a straightforward way to display messages, alerts, and other interactive content to users.

## Features
- **Simple API**: Easy to use and integrate into any web project.
- **Customizable**: Customize the appearance and behavior of the pop-ups.
- **Responsive**: Works well on both desktop and mobile devices.

## Usage
1. **Include the Script**: Add the `jsPopUp.js` script to your HTML file.
   ```html
   <script src="jsPopUp.js"></script>
   ```

2. **Create a Pop-Up**: Use the `jsPopUp.show` method to display a pop-up.
   ```javascript
   jsPopUp.show({
       title: "Hello",
       message: "This is a pop-up message!",
       buttons: [
           { text: "OK", onClick: function() { jsPopUp.hide(); } }
       ]
   });
   ```

## Example
Here is a simple example of how to use the jsPopUp script.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>jsPopUp Example</title>
    <script src="jsPopUp.js"></script>
</head>
<body>
    <button onclick="showPopup()">Show Pop-Up</button>

    <script>
        function showPopup() {
            jsPopUp.show({
                title: "Welcome",
                message: "Welcome to jsPopUp!",
                buttons: [
                    { text: "Close", onClick: function() { jsPopUp.hide(); } }
                ]
            });
        }
    </script>
</body>
</html>
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.