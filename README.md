# Differential Power Analysis of AES

You are provided with power measurements from a smart card performing AES encryption. The encryption was run 100 times, and a power trace was recorded for each run. All required files are included in the `dpa_student_v2.zip` archive.

## Files

| File | Description |
| --- | --- |
| `traces.bin` | Measured trace samples stored consecutively as binary values, with one byte per sample. |
| `traceLength.txt` | Text file containing the length of a single trace. |
| `plaintext.txt` | Plaintext blocks in hexadecimal, one block per line, with bytes separated by spaces. |
| `ciphertext.txt` | Ciphertext blocks in the same format as `plaintext.txt`. |
| `dpa_student.ipynb` | Jupyter notebook with a solution skeleton and useful code. |
| `dpa_bi-hwb_student.nb` (or similar) | Mathematica notebook with a solution skeleton and useful code, for those who prefer Mathematica to Python. |

## Assignment

Complete either the Jupyter or Mathematica notebook:

1. Plot one or a few complete power traces.
2. Select the portion of the traces that is most relevant to DPA, referring to the lecture on side-channel attacks.
3. Update the program to load only the relevant portions of all traces.
4. Extend the program to recover the first byte of the key.
5. Plot the correlation over time for the correct key-byte hypothesis and observe the correlation peaks.
6. Plot and compare the correlation for an incorrect key-byte hypothesis.
7. Extend the code to recover the complete key.
8. Verify the key using a plaintext/ciphertext block pair. You may use an online AES calculator; if you do, document the verification with a note, link, screenshot, or similar evidence.

## Submission

Demonstrate your solution and upload it to GitLab. You do not need to upload the large `traces.bin` file.