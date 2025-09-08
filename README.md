# Symfony AssetMapper Test Project

This is a fresh Symfony 7.1 project with AssetMapper configured and ready for development.

## Setup

The project has been created with the following components:

- **Symfony 7.1** - Latest stable version
- **AssetMapper** - Modern asset management without Webpack/Node.js
- **Basic template structure** - Ready for development

## Project Structure

```
├── assets/                 # Asset files (JS, CSS, images)
│   ├── app.js             # Main JavaScript entry point
│   └── styles/
│       └── app.css        # Main stylesheet
├── config/
│   └── packages/
│       └── asset_mapper.yaml  # AssetMapper configuration
├── importmap.php          # Import map configuration
├── src/
│   └── Controller/        # Controllers
├── templates/             # Twig templates
│   ├── base.html.twig     # Base template with AssetMapper integration
│   └── home/
│       └── index.html.twig # Home page template
└── public/                # Web root
```

## AssetMapper Configuration

- **Assets path**: `assets/`
- **Entry point**: `app.js`
- **Missing import mode**: `strict` (development), `warn` (production)

## Development Server

The development server is configured and ready to run:

```bash
symfony server:start
```

Visit: https://127.0.0.1:8001

## AssetMapper Commands

- `php bin/console debug:asset-map` - View mapped assets
- `php bin/console importmap:require <package>` - Add npm packages
- `php bin/console importmap:update` - Update import map

## Next Steps

This project is ready for:
- Adding Preline UI components
- Integrating Tailwind CSS
- Building custom JavaScript modules
- Adding more controllers and templates

No additional integration has been performed - this is a clean, default AssetMapper setup.
