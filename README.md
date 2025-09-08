# Symfony AssetMapper + Preline UI Project

This is a Symfony 7.1 project with AssetMapper and Preline UI fully integrated and ready for development.

## Setup

The project has been created with the following components:

- **Symfony 7.1** - Latest stable version
- **AssetMapper** - Modern asset management without Webpack/Node.js
- **Preline UI 3.2.3** - Modern UI component library
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
- **Preline UI**: Installed via `importmap:require preline`

## Preline UI Integration

Preline UI has been installed and configured following AssetMapper best practices:

1. **Installation**: `php bin/console importmap:require preline`
2. **Import**: Added to `assets/app.js` with `import 'preline'`
3. **Initialization**: Auto-initialization on DOM ready
4. **Components**: Sample components in home template

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

## Testing the Integration

Visit the application at https://127.0.0.1:8001 to see:
- Preline UI components in action
- Responsive design with Tailwind CSS classes
- JavaScript initialization working
- AssetMapper serving assets correctly

## Next Steps

This project is ready for:
- Building custom Preline UI components
- Adding more controllers and templates
- Integrating additional npm packages via AssetMapper
- Customizing Preline themes and components

The integration is complete and follows Symfony AssetMapper best practices.
