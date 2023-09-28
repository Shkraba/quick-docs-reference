# Cron

A CRON expression is simply a string consisting of six fields that each define a specific unit of time. 

They are written in the following format:

```
{second} {minute} {hour} {day} {month} {day of the week}
```

---

## Values

The following values are allowed within each date/time unit placeholder.

| Field          | Allowed Values | Description                       |
| -------------- | -------------- | --------------------------------- |
| {second}       | 0-59           | Trigger every {second} second(s)  |
| {minute}       | 0-59           | Trigger every {minute} minute(s)  |
| {hour}         | 0-23           | Trigger every {hour} hour(s)      |
| {day}          | 1-31           | Trigger every {day} day(s) of month |
| {month}        | 1-12           | Trigger every {month} month(s)    |
| {day of week}  | 0-6            | MON-SUN Trigger on specific {day of week} |

---

## Special Characters

Additionally, you can also use the following special characters to build more advanced expressions:

| Special Character | Description                     |
| ----------------- | ------------------------------- |
| `*`               | Trigger on tick of every time unit |
| `,`               | List separator                   |
| `–`               | Specifies a range                |
| `/`               | Defines an increment             |

---

## Examples

- `0 * * * * *` - Executes every minute
- `0 0 * * * *` - Executes every hour
- `0 0 0 * * *` - Executes every day
- `0 0 0 0 * *` - Executes every month
- `0 0 0 1 1 *` - Executes on the first day of January each year
- `30 20 * * SAT` - Executes at 08:30 PM every Saturday
- `30 20 * * 6` - Executes at 08:30 PM every Saturday
- `0 */5 * * * *` - Executes every five minutes
- `0 0 8-10/1 * * *` - Executes every hour between 8 AM and 10 AM


## Adding a New Cron Job

To add a new Cron job in Linux, you can use the `crontab` command. Here's how you can add a job that runs a script every day at 3:30 PM:

1. Open your terminal.

2. Edit your Cron jobs by running:

```bash
crontab -e
```

```bash
30 15 * * * /path/to/your/script.sh
```