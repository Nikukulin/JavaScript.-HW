 # Java Script. HomeWork_2


 ```js

    function check_email(test_email) {
        if (typeof test_email !== "string") {
            return [false,"String type error!"];
        }

    if (test_email.value === '') {
        return [false,"Empty string"];
    }
    if (test_email.length < 5) {
        return [false,"The string is too short!"];
    } else if (test_email.length > 64) {
        return [false,"The string is too long!"];
    }
    
    if (test_email.search(/[A-Z,А-Я]/) === -1) {
        return [false,"Enter at least one uppercase letter!"];
    }
    if (test_email.search(/[a-z,а-я]/) === -1) {
        return [false,"Enter at least one letter in lowercase!"];
    }
    if (test_email.search(/[@]/) === -1) {
        return [false,"Enter at least one character @"];
    }
    }
    test_email = "Qwertyshmerty123@mail.ru"
console.log(check_email(test_email))
```