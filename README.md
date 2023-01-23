<!DOCTYPE html>
<html lang="ru">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <?php
    echo 'Основные математические операции' . '<br>';
    $x = 10;
    $y = 20;
    echo '10 + 20 = '.$x + $y .'<br>';
    echo '10 - 20 = '.$x - $y .'<br>';
    echo '10 * 20 = '.$x * $y .'<br>';
    echo '10 / 20 = '.$x / $y .'<br>'.'<br>';
    ?>
    <?php
    echo 'Вариант 3' . '<br>';
    function am($n)
    {
        $b = null;
        if ($n == 1) {
            return 1;
        }
        if ($n > 1) {
            return (int)am($n/2) + 1;
            
        }
        if ($n < 1) {
            return ('*кхм-кхм, кажется вы ввели n < 1*');
        }
    }
    echo 'При заданном n число a = ', am(5);
    ?>
</body>

</html>
