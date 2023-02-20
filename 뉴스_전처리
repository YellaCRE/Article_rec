def text_preprocessing(text):
    #괄호안제거
    text = re.sub(r'\([^)]*\)' , '', string=text)
    text = re.sub(r'\[[^)]*\]' , '', string=text)
    text = re.sub(r'\{[^)]*\}' , '', string=text)
    text = re.sub(r'\≪[^)]*\≫' , '', string=text)
    text = re.sub(r'\<[^)]*\>' , '', string=text)

    #특정 문자제거
    table = str.maketrans('[$%&()*+,-/:;<=>^_{}~@#]©', "                         ")
    text = text.translate(table)

    #이메일주소
    pattern = '(\[a-zA-Z0-9\_.+-]+@\[a-zA-Z0-9-\]+.\[a-zA-Z0-9.\]+)'
    text = re.sub(pattern=pattern, repl=' ', string=text)

    #url 제거
    pattern_url = '(http|ftp|https)://(?:[-\w.]|(?:\[da-fA-F]{2}))+'
    text = re.sub(pattern=pattern_url, repl='', string=text)

    #\r, \n제거하기
    text = re.sub('[\r|\n]', repl ='', string=text)

    #nbsp 반복
    text = re.sub("nbsp", " ", string = text)

    #... 제거
    text = text.replace('…',' ')
    text = text.replace('···',' ')
    text = text.replace('..',' ')
    
    return text
