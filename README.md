# stress-testing

## Prerequisite
- Jmeter

## About this project:
This is a random API from where we can get the list of the users. No error were found till 10000 loads in 1800 seconds after executing the stress test. So the actual TPS will be 10000/1800 = 5.555555555555556 . And the capacity is 5.555555555555556 *12*60*60 = 240,000. Initial condition was to check TPS for 120000 loads in 12 hours. Where our expexted and actual TPS was 2.7777777778.

## How to run this project:
-You need to set path of java home and jmeter home in environment variables.
- clone this project
``` https://github.com/mashruf/stress-testing ```
- In the source root project, give the following command:
``` jmeter -n -t stress-test.jmx -l stress-test.csv -e -o report ```

![stress test](https://github.com/mashruf/stress-testing/assets/50927464/f176e2a2-64d9-4d67-a1ff-5902b131811d)

![Capture](https://github.com/mashruf/stress-testing/assets/50927464/9eb030ae-b3f7-4723-a71e-15341e711381)
