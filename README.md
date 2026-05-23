# Anonymous Children Story Dataset

This repository provides the processed dataset used in our submission.

## Contents

- `pages_pretty_by_storyname/`: page-level story files (one JSON per story), grouped by age bucket.
- `stories_merged_per_file/`: story-level merged files (one JSON per story), grouped by age bucket.
- `age_distribution_summary.json`: age-bucket counts over the released dataset.
- `dataset_paper_stats_summary.json`: dataset statistics used in the paper.

## Data Format

### Page-level file (`pages_pretty_by_storyname/.../*.json`)
Each file is a list of page records with fields such as:
- `title_zh`, `title_en`
- `target_age`
- `source_type`, `source_file`
- `source_page`, `page_text_ocr_zh`, `page_text_en`, `summary_zh`

### Story-level file (`stories_merged_per_file/.../*.json`)
Each file is one merged story record with fields such as:
- `title_zh`, `title_en`, `target_age`
- `source_type`, `source_file`, `page_count`
- `full_text_zh`, `full_text_en`, `full_summary_zh`

## License

This dataset release is provided under **CC BY 4.0**.
