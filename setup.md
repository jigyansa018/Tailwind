## How to set a tailwind css

Step - 1: Run this command in terminal

        npm install -D tailwindcss(1st run this)
        npx tailwindcss init(2nd run this)

Step - 2: Update tailwind.config.js file to include this line:

        content: ["*.html"],(to match all html file)
        content: ["./src//*.{html,js}"],(this is to match all html and js file)

Step-3: Cretae a src folder under that create a input.css file then add this

        @tailwind base;
        @tailwind components;
        @tailwind utilities;

Step - 4: link the output.css file in to your html file

Step - 5: Run this Command

        npx tailwindcss -i ./src/input.css -o ./src/output.css --watch