## String#bracket

    require 'facets/string/bracket'

    'X'.bracket('#').assert == '#X#'
    'X'.bracket('x','!').assert == 'xX!'
    'X'.bracket('{','}').assert == '{X}'
    'X'.bracket('<').assert == '<X>'
    'X'.bracket('(').assert == '(X)'
    'X'.bracket('[').assert == '[X]'
    'X'.bracket('{').assert == '{X}'

## String#bracket!

    a = 'X' ; a.bracket!('#')
    a.assert == '#X#'

    a = 'X' ; a.bracket!('x','!')
    a.assert == 'xX!'

    a = 'X' ; a.bracket!('{','}')
    a.assert == '{X}'

    a = 'X' ; a.bracket!('<')
    a.assert == '<X>'

    a = 'X' ; a.bracket!('(')
    a.assert == '(X)'

    a = 'X' ; a.bracket!('[')
    a.assert == '[X]'

    a = 'X' ; a.bracket!('{')
    a.assert == '{X}'

