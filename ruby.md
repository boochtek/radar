Ruby
====

* [Pretty Ruby](https://github.com/jonahx/pretty_ruby) - gem to extend Enumerable/Array in beautiful ways
    * Uses refinements instead of monkey-patching
    * Great article: https://dzone.com/articles/making-ruby-yours
* Bundler-audit
* [Roo](https://github.com/roo-rb/roo) - gem to read/write various spreadsheet formats (Excel, OpenOffice, CSV)
    * For old Excel XLS files and Google spreadsheet, add roo-xls and roo-google gems
* [rb](https://github.com/mcandre/rubycheck) - use Ruby as a command-line tool
    * Use Ruby more like Perl -pie
* Property-based testing libraries (haven't tried any of them yet)
    * [Rantly](https://github.com/rantly-rb/rantly)
    * [Hypothesis](https://github.com/HypothesisWorks/hypothesis/tree/master/hypothesis-ruby)
    * [RubyCheck](https://github.com/mcandre/rubycheck)
* [PgSearch](https://github.com/Casecommons/pg_search) - full-text search

## Testing

## Debugging

- Pry-byebug - allows setting breakpoints

## Static Analysis

- [Rubocop](https://rubocop.org/)
    - style checker (linter) and formatter based
    - based on [Ruby Style Guide](https://rubystyle.guide/)
- [Reek](https://github.com/troessner/reek)
    - detects code smells
- [bundler-audit](https://github.com/rubysec/bundler-audit)
    - checks for vulnerable versions of gems
