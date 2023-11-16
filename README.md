# Abaqira Academy Website

This repository contains the code for the Abaqira Academy website, which provides information about the academy and its offerings for primary and kindergarten education in Addis Ababa.

## Usage

To use this code, follow the instructions below:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/ahmedonour/abaqira-academy.git
   ```

2. Navigate to the project directory:

   ```bash
   cd abaqira-academy
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Run the application:

   ```bash
   npm run dev
   ```

   This will start the development server, and you can view the website by navigating to [http://localhost:5000](http://localhost:5000) in your web browser.

## Code Structure

The main entry point for the application is the `index.svelte` file. This file imports the `Hero` component from the `component` directory and includes necessary metadata in the `<svelte:head>` section.

```javascript
<script>
	import Hero from '../component/Hero.svelte';
</script>

<svelte:head>
	<meta charset="UTF-8">
    <meta name="description" content="Abaqira Academy - Providing Quality Education for Primary and Kindergarten Students in Addis Ababa">
    <meta name="keywords" content="Primary School, Kindergarten, Education, Addis Ababa, Abaqira Academy">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Abaqira Academy - Quality Primary and Kindergarten Education in Addis Ababa</title>
</svelte:head>

<main>
	<Hero />
</main>

<style>
	/* Custom styles can be added here */
</style>
```

## Styles

The `style` block within the `index.svelte` file contains custom styles for the application. You can modify these styles or add additional styles as needed.

```css
<style>
	/* main{
        display: grid;
        place-items: center;
    } */
</style>
```

Feel free to customize the styles according to your design preferences.

## License

This code is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code for your own educational purposes or other non-commercial projects.

If you have any questions or issues, please feel free to [open an issue](https://github.com/your-username/abaqira-academy/issues) on the repository.

Thank you for using the Abaqira Academy website code!
