# Committed dataset

**Source dataset:** NAVER CLOVA CORD-v2 receipt parsing

**Selection:** Source subset: first 20 train receipts and first 10 test receipts exposed by the publisher dataset viewer. All OCR words/categories and structured ground-truth fields for these receipts are included, with API-exported JPEG image copies.

**Data license:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). This applies to the data, independently of the project code.

## Sources

- https://github.com/clovaai/cord
- https://huggingface.co/datasets/naver-clova-ix/cord-v2
- https://datasets-server.huggingface.co/first-rows?dataset=naver-clova-ix/cord-v2&config=default&split=train
- https://datasets-server.huggingface.co/rows?dataset=naver-clova-ix/cord-v2&config=default&split=test&offset=0&length=10

## CSV files

| File | Rows | Bytes |
|---|---:|---:|
| [cord_receipts.csv](raw/cord_receipts.csv) | 30 | 210,277 |
| [cord_words.csv](raw/cord_words.csv) | 830 | 63,757 |
| [cord_fields.csv](raw/cord_fields.csv) | 460 | 18,367 |

Attribution: Seunghyun Park and NAVER CLOVA CORD team, CORD: A Consolidated Receipt Dataset for Post-OCR Parsing (2019). Replaces FUNSD with an explicitly licensed publisher release. This is receipt parsing, not an invoice or form-question benchmark. Source revision: 7f0115a4b758a71d6473b8d085751692da2fef98. All original ground-truth JSON is preserved in the receipt CSV; field_path is a derived join key. Source split labels are unchanged. The 30-receipt subset is an initial development sample, not the full benchmark or sufficient evidence of broad layout generalization. Image geometry is verified against the viewer's reported dimensions.

The CSV files contain published observations or their documented format conversion; no training records were invented. Source formats and raw CSV exports are distinguished by the manifest. File checksums and schemas are recorded in [csv-manifest.json](csv-manifest.json).
