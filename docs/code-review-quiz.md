# Code review

In this section, try to find what is wrong with each code sample.

## Alarm clock

Write a script which will trigger an action every day at the same time. The input is information about hour,
minute and second when it should be triggered. The input is in format `hour:minute:second`.

```php
<?php
if ($argc !== 2)
{
	echo "Usage script.php <hour:minute:second>";
	exit;
}

$targetTime = $argv[1];
list ($h, $i, $s) = explode(':', $argv[1]);

while (true) {
	if ($h === date('H')) {
		if ($i === date('i')) {
			if ($s === date('s')) {
				echo "Wake up";
				// trigger additional action
			}
		}
	}
}

```

<details>

<summary>Solution</summary>

Solution is not yet provided, it's up to you to try to solve it.

</details>
