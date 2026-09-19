## How to setup Tailwind CSS

Step 1: Run the following Commands
```
npm install tailwindcss @tailwindcss/cli
npx tailwindcss init
```

Step 2: Create src/input.css to include:
```
@import "tailwindcss";
```

Step 3: Create tailwind.config.js file.. 
```
Code :
/** @type {import('tailwindcss').Config} */
module.exports = {
    content: [],
    theme: {
        extend:{},
    },
    plugins: [],
}
```

Step 4: Now, Run this command to create output.css.
```
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```

Step 5: Include the src/output.css file to your html.
```
<link rel="stylesheet" href="src/output.css">
```

Step 6: Now, Your Tailwindcss is done to run in your html program.