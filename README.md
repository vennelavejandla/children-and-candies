length = len(string)
vowels = {'A', 'E', 'I', 'O', 'U'}
vowel_word_idx_cnt = []
consonant_word_idx_cnt = []

for i, char in enumerate(string):
        if char in vowels:
            vowel_word_idx_cnt.append(length-i)
        else:
            consonant_word_idx_cnt.append(length-i)
    
vowel_word_count = sum(vowel_word_idx_cnt)
consonant_word_count = sum(consonant_word_idx_cnt)
if vowel_word_count > consonant_word_count:
        print('Kevin', vowel_word_count )
elif consonant_word_count > vowel_word_count:
        print('Stuart', consonant_word_count )
    else:
        print('Draw')
