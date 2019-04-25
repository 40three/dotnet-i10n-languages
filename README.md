# dotnet-i10n-languages
Contains language names in all languages using cldr data. While it's easy to show a list of languages in English or in it's native name, there's no data to show all languages is a specified language. That's what this nuget package provides.

# How to Use

## Example

Namespace: Fortythree.I10n.Languages

     var languages = Loader.Load("de-DE");

     var name = languages["de"].LanguageName;
     // name = "Deutsch"

## Data

Loader returns a `Dictionary<string, I10nLanguage>`

    public class I10nLanguage
    {
        // de-DE
        public string Code { get; }
        
        // Deutsch (Deutschland)
        public string Name { get; }
        
        // Deutsch
        public string LanguageName { get; }
        
        // Deutschland
        public string TerritoryName { get; }
    }

# Project Sources
For now, this repository is a placeholder intended for issue tracking and documentation. We use our internal git repository to be able to use existing ci infrastructure.
