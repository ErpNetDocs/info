# Multi-language support
 
## Description
Many string attributes in @@name support saving the data in multiple languages. These attributes are called Multi-language Strings.

For example, the Product Name of a Product can be entered in many languages simultaneously.

When visualizing the data, the correct language version of the string is displayed automatically by the system, depending on the current user language.


> [!NOTE]
> For reports, the report designer can specify whether to use the current user language or always use a fixed language.
> For example, for a Portuguese invoice, one would require that the labels and data are always displayed in Portuguese.


## Entering data in multiple languages

The client applications of @@name usually allow the following abilities regarding multi-language strings:
- Enter the string in many languages
- Transliterate a string from one language to another (or all)
- Translate a string from one language to another (or all)

When entering translations for a multi-language string, the client application usually displays a table with cells for each language translation, similar to this:

| Language | Value |
| ---- | ----- |
| EN: | Toothpaste |
| DE: | Zahnpasta |

Depending on the client application, translation can sometimes also be automated. Some client applications support using an online service, like Google Translate to automatically translate a string to other languages. Translation is better suited to Description and Notes attributes.


## Transliteration

Transliteration is the process of translating one language version of a string to another, based on the sounding of the string. Transliteration works great for person and company names and addresses. It allows branch offices to work in their local language and reports can still be shown in the corporate language.

For example, the Russian word "Иван" would be transliterated in English as "Ivan".

Transliteration works in two ways - manual and automatic.


### Manual transliteration

"Manual" transliteration is actually automatic, but is initiated manually while editing the different language versions of a multi-language string. While editing multi-language string, the client application usually provides a function button, which transliterates the current language version to other languages.


### Automatic transliteration

Automatic transliteration occurs when the system needs to display some a multi-language string in some language, but that specific language translation is not saved in the database.

For example, suppose one employee works in a branch office in Russia and enters "Иван" as a person first name. The database saves only the Russian language version. Then another employee at a UK location requests to see the first name of the same person. The system would automatically transliterate the string and display it as "Ivan".

> [!NOTE]
> Transliteration works optimally between Latin and Cyrillic.
