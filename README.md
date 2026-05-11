# Time Recording Assessor

Static GitHub Pages app for reviewing time recording CSVs.

## Workflow

1. Open Step 1: Review and export CSV.
2. Import a time recording CSV.
3. Review Project, Timecode and Comment.
4. Add or accept suggested local tags.
5. Export the reviewed CSV.
6. Store reviewed CSVs in one laptop folder.
7. Open Step 2: Review historic CSVs.
8. Choose or sync that folder to load historic reviewed entries and reusable rules.

## Saved tag suggestions and rules

- When you export a reviewed CSV, the app learns suggestions from local tags you applied.
- Suggestions are based on Project + Timecode.
- On the next import, matching rows show suggested tags.
- Suggestions are not applied automatically. Use the row-level Use button or Apply visible suggestions.
- Use Do not suggest to suppress a suggested tag for that Project + Timecode.
- Tag override rules and tag suggestion rules are stored in the historic CSV folder as `time-recording-assessor-rules.json`.
- Syncing the historic folder loads reviewed CSVs and the rules file.
- Export reviewed CSV to historic folder writes both the reviewed CSV and the rules file.
- If you use Download reviewed CSV, save the CSV into your historic folder and use Save rules to folder to write the current rules file.

## Notes

- The app is a single static HTML file and needs no build step.
- Historic review reads reviewed CSV files from the folder you choose.
- Browser folder access works best in Chrome or Edge.
- GitHub Pages cannot silently read an arbitrary folder path unless the browser has granted permission.
