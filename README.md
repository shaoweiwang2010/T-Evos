# T-Evos

T-Evos: A Large-Scale Longitudinal Study on CI Test Execution and Coverage Evolution

This GitHub repository is created to showcase our dataset. Please kindly find our complete dataset on code coverage and test results at [T-Evos Zenodo repository](https://zenodo.org/record/5500821)

## Description

T-Evos is a dataset on test result and coverage evolution, covering 6,495 consecutive commits across 12 open-source Java projects.

Due to the large volume of data, we are still looking for the best way to share them. 🤔 More updates to come! 

💬 v0.1.0: added some sample data to help illustrate our dataset, please kindly find our full dataset on code coverage and test results at https://zenodo.org/record/5500821

## Data summary
We summarize the dataset below.

| Projects               | Commits  | Commits with failure (failure ratio) | Total test failure instances | Flaky  | Non-flaky | New test failures | Resolved test failures |
|------------------------|----------|--------------------------------------|------------------------------|--------|-----------|-------------------|------------------------|
| commons-cli            | 558      | 121 (22%)                           | 183                          | 53     | 130       | 60                | 60                     |
| commons-codec          | 709      | 340 (48%)                           | 4,351                        | 1,105  | 3,246     | 58                | 47                     |
| commons-compress       | 337      | 182 (55%)                           | 3,812                        | 3,697  | 115       | 192               | 191                    |
| commons-csv            | 805      | 123 (16%)                           | 247                          | 229    | 18        | 32                | 32                     |
| commons-math           | 117      | 113 (97%)                           | 1,003                        | 1,001  | 2         | 2                 | 2                      |
| gson                   | 310      | 310 (100%)                          | 7,652                        | 5,808  | 1,844     | 53                | 43                     |
| jackson-core           | 453      | 344 (76%)                           | 2,672                        | 162    | 2,510     | 99                | 97                     |
| jackson-dataformat-xml | 203      | 153 (76%)                           | 156                          | 4      | 152       | 10                | 10                     |
| jfreechart             | 439      | 342 (78%)                           | 1,253                        | 635    | 618       | 27                | 13                     |
| junit4                 | 596      | 321 (54%)                           | 386                          | 347    | 39        | 35                | 35                     |
| jsoup                  | 990      | 42 (5%)                             | 66                           | 0      | 66        | 23                | 23                     |
| fastjson               | 978      | 333 (35%)                           | 553                          | 10     | 543       | 230               | 230                    |
| Total                  | 6,495    | 2,724 (42%)                         | 22,334                       | 13,051 | 9,283     | 821               | 783                    |


## Structure
We present T-Evos repository structure below.

```
│
├── code_changes
│	 └── code_changes.json 		(code changes)
│
├── coverage
│   ├── 0303dc (commit hash)
│   │   └── ExampleTest.json 	(coverage)
│   └─ ...
│
├── build_logs
│   └── 0303dc_out.txt 			(build logs)
│
├── test_status
│   ├── 0303dc (commit hash)
│   │   └── ExampleTest.log 	(test status, test stack traces)
│   └─ ...
```
