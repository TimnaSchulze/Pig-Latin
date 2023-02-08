Describe: pigLatin

Test: "It will split the word into an array of letters."
Code pigLatin("word");
Expected Output: 'w', 'o', 'r', 'd'

function pigLatin() {
  const string = "word";
  string.split('');
}


Test: "It will output the first letter of the word."
Code pigLatin("word");
Expected Output: "w"

// return the first letter of a word
function pigLatin() {
  const word = "word";
  let firstLetter = word.charAt(0);
}


Test: "It will check the first letter of each word for a vowel (a, e, i, o, u)."
Code: pigLatin("orange cat");
Expected Output: o

Test: "It ignores non-alphabetical characters."
Code: pigLatin("*&$92%");
Expected Output: null

Test: "It will add "way" to the end of words that begin with a vowel."
Code: pigLatin("orange");
Expected Output: orangeway

Test: "It will check the first letter of each word for a consonant."
Code: pigLatin("orange cat");
Expected Output: cat

Test: "It will recognize the consonants before the first vowel in a word that begins with a consonant."
Code: pigLatin("shoes");
Expected Output: sh

Test: "It will move the consonants before the first vowel in a word that begins with a consonant to the end of the word."
Code: pigLatin("shoes");
Expected Output: oessh

Test: "It will add "ay" to the end of the reconstructed word that began with a consonant(s)."
Code: pigLatin("oessh");
Expected Output: oesshay

Test: "It will check for a "qu" pair at the beginning of a word."
Code: pigLatin("queen");
Expected Output: qu

Test: "It will move "qu" pair from the beginning of a word to the end."
Code: pigLatin("queen");
Expected Output: eenqu

