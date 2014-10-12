# Module Documentation

## Module Data.String

### Types

    newtype Char


### Values

    charAt :: Number -> String -> String

    charAt' :: Number -> String -> Maybe Char

    charCodeAt :: Number -> String -> Number

    charCodeOf :: Char -> Number

    drop :: Number -> String -> String

    fromArray :: [Char] -> String

    fromCharCode :: Number -> String

    fromCharCode' :: Number -> Char

    indexOf :: String -> String -> Number

    indexOf' :: String -> Number -> String -> Number

    joinWith :: String -> [String] -> String

    lastIndexOf :: String -> String -> Number

    lastIndexOf' :: String -> Number -> String -> Number

    length :: String -> Number

    localeCompare :: String -> String -> Number

    replace :: String -> String -> String -> String

    split :: String -> String -> [String]

    take :: Number -> String -> String

    toArray :: String -> [Char]

    toLower :: String -> String

    toUpper :: String -> String

    trim :: String -> String


## Module Data.String.Regex

### Types

    data Regex :: *

    type RegexFlags  = { unicode :: Boolean, sticky :: Boolean, multiline :: Boolean, ignoreCase :: Boolean, global :: Boolean }


### Type Class Instances

    instance showRegex :: Show Regex


### Values

    flags :: Regex -> RegexFlags

    match :: Regex -> String -> [String]

    parseFlags :: String -> RegexFlags

    regex :: String -> RegexFlags -> Regex

    renderFlags :: RegexFlags -> String

    replace :: Regex -> String -> String -> String

    replace' :: Regex -> (String -> [String] -> String) -> String -> String

    search :: Regex -> String -> Number

    source :: Regex -> String

    test :: Regex -> String -> Boolean