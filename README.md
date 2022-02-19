# entropy-secrets-finder
Script to find leaked secrets in files (JS, GH, etc.)

Entropy analysis is very powerful in discovering leaked secrets like API keys, however the false positive rate is much too high to be deemed realistic. I've taken some steps to reduce these false positives with tricks like checking character capilization ratios. Lexically in English a word consists mainly of lower case letters, but in regards to computer generated letters it either IS or IS NOT capitilized. This allows us to add a soft-check to determine if a string is randomly generated.
