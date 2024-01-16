This script processes the folder generated by PlatEMO as result of an experiment, and it generates a `CSV` file (plain text) combining
all data of each run for each algorithm, problem, and metric. This generated file is useful to have all metric values
for easy analysis on Excel, Google Spread Sheet, Numbers, or others.

By default, when performing any experiment, PlatEMO generates a folder containing the `Setting.mat` file and a folder for
each algorithm under analysis. For each algorithm, PlatEMO creates a folder where it stores a matlab file (with
extension `.mat`) for each run, containing different metric values.

The script assumes that `.mat` file names follow the format given by PlatEMO for experiments. For instance, the file
`GWASFGA_DTLZ1_M3_D7_1.mat` is generated by PlatEMO when running the GWASFGA algorithm, over the DTLZ1 problem with three
objective functions, and seven decision variables. The last number, before the `.mat` extension, refers to the run number.

The script has been successfully tested on PlatEMO 4.5.
