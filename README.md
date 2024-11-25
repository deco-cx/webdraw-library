# Webdraw Library prompts

The **Webdraw Library** allows developers to create and manage custom prompts by defining them in standalone HTML files. This guide provides instructions and best practices for adding prompts to the library.

## Adding a prompt

### 1. Create an HTML File
Each prompt is defined as a single HTML file. Name the file descriptively based on the prompt's purpose (e.g., `my_custom_prompt.html`).

### 2. Define the Metadata
Add metadata tags to the `<head>` section of your HTML file. These tags define the prompt's properties and functionality.

#### Example prompt File
```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Custom prompt</title>
  
  <!-- Short description of the prompt -->
  <meta name="description" content="This custom prompt adds * capabilities to your application.">
  
  <!-- SVG icon for the prompt -->
  <meta name="icon" content="<svg xmlns='http://www.w3.org/2000/svg' width='48' height='48' viewBox='0 0 28 28' fill='none'><path fill='#ED225D' stroke-miterlimit='10' d='M16.909,10.259l8.533-2.576l1.676,5.156l-8.498,2.899l5.275,7.48 l-4.447,3.225l-5.553-7.348L8.487,26.25l-4.318-3.289l5.275-7.223L0.88,12.647l1.678-5.16l8.598,2.771V1.364h5.754V10.259z'></path></svg>">
  
  <!-- URL for examples or documentation -->
  <meta name="examples" content="https://example.com/documentation/prompt-usage">
  
  <!-- Custom instructions for the AI -->
  <meta name="metadata" content="Set of custom instructions that will be added to the prompt to influence the result of the generated output.">
</head>
</html>

</html>
```

### 3. Metadata Tags

| **Tag Name**       | **Description**                                                                            |
|---------------------|--------------------------------------------------------------------------------------------|
| `description`      | Short description of the prompt's functionality.                                           |
| `icon`             | SVG icon that represents the prompt. When embedded in the `content` attribute, all attributes inside the SVG must use single quotes (`'`).                              |
| `examples`         | URL pointing to usage examples, documentation, or a demo of the prompt.                    |
| `metadata`         | Set of custom instructions that will be added to the prompt to influence the result of the generated output.                     |




