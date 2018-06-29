# Words Count
Words count for multi-languages paragraph mixed with numbers and punctuations.   
One rule apply to all.  
  
[See Test Case](https://byn9826.github.io/words-count/)  
  
Install
--
```
npm i words-count
```

Example
--
```
var wordsCount = require('words-count');  
console.log(wordsCount('Hello World'));  
```
  
Why use this
--
words_to_be_count = 'Hello “世界”';  
words-count.js -> 3  
  
words_to_be_count.length -> 10  
words_to_be_count.split(' ').length -> 2  
Countable.js -> 2  
PHP str_word_count(words_to_be_count) -> 1  
PHP mb_strlen(words_to_be_count) -> 10  
Office Word -> 5  

Special Rule
--
1. Numbers count as 1 word  
2. Words connected by '-' count as 2 words  

Test Case
--
<b>Original Content:</b>  
Google's free service instantly translates words, phrases, and web pages between English and over 100 other languages.  
<b>Basic Test Content:</b>  
Translate original content into target language by Google Translate.  
<b>Test Case Coverage:</b>  
  English, Chinese, Chinese-Traditional, Japanese, Korean, French,  German,  
  Italian, Spanish, Portuguese, Russian, Ukrainian, Arabic, Hebrew, Afrikaans,  
  Albanian, Amharic, Armenian, Azerbaijani, Basque, Belarusian, Bengali,  
  Bulgarian, Bosnian, Catalan, Cebuano, Croatian, Chichewa, Corsican, Czech,  
  Danish, Dutch, Esperanto, Estonian, Filipino, Finnish, Frisian, Greek, Galician,  
  Georgian, Gujarati, Haitian Creole, Hausa, Hindi, Hmong, Hungarian, Icelandic,  
  Igbo, Indonesian, Irish, Javanese, Kannada, Kazakh, Kurdish, Kyrgyz, Latin,  
  Latvian, Lithuanian, Luxembourgish, Macedonian, Malagasy, Malay, Malayalam,  
  Nepali, Norwegian, Polish, Romanian, Serbian, Slovenian, Swedish, Turkish, Welsh  
  Zulu, Maori, Marathi, Mongolian, Pashto, Persian, Punjabi, Scots Gaelic, Sesotho,  
  Shona, Sindhi, Sinhala, Slovak, Somali, Sundanese, Swahili, Tajik, Turkish,  
  Urdu, uzbek, Vietnamese, Xhosa, Yiddish, Yoruba  
<b>Failed/Unknown:</b>
Hawalian, Khmer, Lao, Maltese, Myanmar, Tamil, Thai
  
Reference
--
http://php.net/manual/en/function.str-word-count.php#109733  
https://www.key-shortcut.com/en/writing-systems/%E6%96%87%E5%AD%97-chinese-cjk/cjk-characters-1/
http://jrgraphix.net/r/Unicode/0D00-0D7F