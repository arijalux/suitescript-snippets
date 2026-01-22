# SuiteScript 2.1 Code Snippets

**Author:** Clemen Canaria  
**Email:** ccanaria [at] gmail [dot] com | clemen [at] canariawerx [dot] com  
**Organization:** CanariaWerx

A comprehensive collection of VS Code snippets for NetSuite SuiteScript 2.1 development using ECMA 6 syntax.

## Features

This extension provides code snippets for all major SuiteScript 2.1 script types and common patterns:

### Script Types
- **RESTlet** (`ss21-restlet`) - Complete RESTlet with GET, POST, PUT, DELETE handlers
- **Suitelet** (`ss21-suitelet`) - Suitelet with GET and POST request handling
- **User Event** (`ss21-userevent`) - User Event Script with beforeLoad, beforeSubmit, afterSubmit
- **Map/Reduce** (`ss21-mapreduce`) - Map/Reduce script with all four phases
- **Scheduled Script** (`ss21-scheduled`) - Scheduled Script template
- **Client Script** (`ss21-client`) - Client Script with all event handlers
- **Portlet** (`ss21-portlet`) - Portlet Script template
- **Mass Update** (`ss21-massupdate`) - Mass Update Script template
- **Workflow Action** (`ss21-workflowaction`) - Workflow Action Script template
- **Bundle Installation** (`ss21-bundleinstall`) - Bundle Installation Script template
- **Module** (`ss21-module`) - Reusable module template

### Helper Snippets
- **Search** (`ss21-search`) - Create and execute a search
- **Record Load** (`ss21-record-load`) - Load a record
- **Record Create** (`ss21-record-create`) - Create a new record
- **HTTP Request** (`ss21-http-request`) - Make an HTTP request
- **Try-Catch** (`ss21-try-catch`) - Try-catch block with error handling
- **Console Log** (`ss21-console-log`) - Console log message
- **Console Error** (`ss21-console-error`) - Console error message

## Usage

1. Open a JavaScript file in VS Code
2. Start typing the snippet prefix (e.g., `ss21-restlet`)
3. Press `Tab` or `Enter` to insert the snippet
4. Use `Tab` to navigate through placeholders

## Example

Type `ss21-restlet` and press Tab to insert:

```javascript
/**
 * @NApiVersion 2.1
 * @NScriptType Restlet
 * @author Your Name
 */
define([], () => {
    
    /**
     * GET request handler
     * @param {Object} requestParams - Request parameters
     * @returns {Object} Response object
     */
    const get = (requestParams) => {
        try {
            
            return { success: true, data: {} };
        } catch (e) {
            return { success: false, error: e.message };
        }
    };
    
    // ... more handlers
    
    return { get, post, put, delete: doDelete };
});
```

## Features

- ✅ ECMA 6 syntax (arrow functions, const/let, destructuring)
- ✅ JSDoc annotations for better IntelliSense
- ✅ No log module dependencies (uses console for client-side)
- ✅ Tab stops for quick navigation
- ✅ Proper error handling patterns
- ✅ @author tag for attribution

## Requirements

- Visual Studio Code 1.80.0 or higher
- JavaScript language support

## Installation

### Method 1: From VS Code Marketplace (Recommended)
1. Open VS Code
2. Go to Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X` on Mac)
3. Search for "SuiteScript 2.1 Code Snippets"
4. Click **Install**
5. Reload VS Code if prompted

### Method 2: From VSIX File
1. Download the `.vsix` file from the releases page
2. Open VS Code
3. Go to Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X` on Mac)
4. Click the "..." menu (three dots) at the top of the Extensions view
5. Select **Install from VSIX...**
6. Navigate to and select the downloaded `.vsix` file
7. Reload VS Code if prompted

### Method 3: From Source (For Development)
1. Clone this repository:
   ```bash
   git clone https://github.com/ccanaria/suitescript-snippets.git
   cd suitescript-snippets
   ```
2. Copy the folder to your VS Code extensions directory:
   - **Windows**: `%USERPROFILE%\.vscode\extensions\suitescript-snippets`
   - **macOS/Linux**: `~/.vscode/extensions/suitescript-snippets`
3. Restart VS Code

## How to Use

### Basic Usage
1. **Open or create** a JavaScript file (`.js`) in VS Code
2. **Type** the snippet prefix (e.g., `ss21-restlet`)
3. **Select** the snippet from the IntelliSense dropdown that appears
4. **Press** `Tab` or `Enter` to insert the snippet
5. **Navigate** through placeholder fields using `Tab`
6. **Fill in** the placeholders with your specific values

### Triggering IntelliSense
If the snippet dropdown doesn't appear automatically:
- Press `Ctrl+Space` (Windows/Linux) or `Cmd+Space` (Mac) to manually trigger IntelliSense
- Start typing the snippet prefix more completely

### Available Snippet Prefixes
All snippets start with `ss21-` followed by the script type or function:

**Script Types:**
- `ss21-restlet` - RESTlet script
- `ss21-suitelet` - Suitelet script
- `ss21-userevent` - User Event script
- `ss21-mapreduce` - Map/Reduce script
- `ss21-scheduled` - Scheduled script
- `ss21-client` - Client script
- `ss21-portlet` - Portlet script
- `ss21-massupdate` - Mass Update script
- `ss21-workflowaction` - Workflow Action script
- `ss21-bundleinstall` - Bundle Installation script
- `ss21-module` - Reusable module

**Helper Functions:**
- `ss21-search` - Search creation and execution
- `ss21-record-load` - Load a record
- `ss21-record-create` - Create a new record
- `ss21-http-request` - HTTP request
- `ss21-try-catch` - Try-catch block
- `ss21-console-log` - Console log
- `ss21-console-error` - Console error

### Tips for Maximum Productivity
- **Enable Tab Completion**: Ensure tab completion is enabled in VS Code settings
  - Go to `File > Preferences > Settings` (or `Code > Preferences > Settings` on Mac)
  - Search for "tab completion"
  - Set `editor.tabCompletion` to `on` or `onlySnippets`
- **View All Snippets**: Type `ss21-` and press `Ctrl+Space` to see all available snippets
- **Customize Snippets**: You can modify snippets in VS Code by going to `File > Preferences > Configure User Snippets > javascript.json`
- **Use Multi-Cursor**: Use `Alt+Click` (Windows/Linux) or `Option+Click` (Mac) to edit multiple placeholders simultaneously

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under a **Custom Source-Available License**.

This means:
- ✅ You can fork this repository and modify it
- ✅ You can use it in your own projects (personal or commercial)
- ✅ You can use the code in your own work
- ❌ You cannot create standalone copies or redistributions
- ❌ You cannot republish this as your own work
- ⚠️ All forks must maintain attribution to the original author
- ⚠️ Public forks must link back to the original repository

See the [LICENSE](LICENSE) file for full details.

## Author

**Clemen Canaria** - [CanariaWerx](https://github.com/canariawerx)  
📧 ccanaria [at] gmail [dot] com | clemen [at] canariawerx [dot] com

## Release Notes

### 1.0.0

Initial release with support for all major SuiteScript 2.1 script types and common patterns.
