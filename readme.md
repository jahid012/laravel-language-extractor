# Laravel Language Extractor

The Laravel Language Extractor is a command-line tool for extracting localization keywords from Laravel PHP source files. It searches through all PHP files in a specified directory and extracts all translation keys used in the `__()` helper function and outputs them to a JSON file.

## Installation

The Laravel Language Extractor is distributed as a binary executable file. Download the binary for your platform from the releases page on GitHub, and place it in your preferred location.

## Usage

```
laravel-lang-extractor <directory-path>
```

The `directory-path` argument specifies the root directory where the PHP files to extract localization keys from are located.

The extracted localization keys are written to a file named `en.json` in the current working directory.

### Example

```
laravel-lang-extractor /path/to/laravel/app
```

This command will search for all PHP files in the `/path/to/laravel/app` directory and extract all localization keys used in the `__()` helper function, and output them to a JSON file named `en.json` in the current working directory.

## Output

The output JSON file contains all localization keys found in the source files, with their values set to the same as the key.

```
{
    "key1": "key1",
    "key2": "key2",
    "key3": "key3"
}
```

## License

The Laravel Language Extractor is released under the MIT License. See the [LICENSE](LICENSE) file for more details.