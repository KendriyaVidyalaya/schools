📚 Kendriya Vidyalaya Schools Dataset
==================================

A comprehensive, regularly-updated dataset of all Kendriya Vidyalaya (KV) schools around the globe, including their codes, names, states, regions, and profiles.

📌 About
-----
This repository provides open data on all Kendriya Vidyalaya schools. The dataset is automatically fetched and refreshed to ensure accuracy. It can be used for research, analysis, applications, or to help parents/students find KVs.

📅 Dataset Structure
-----------------
- raw/schools.json      List of all schools with codes, names, state, and region.
- raw/schools.txt       Plain text list of school names.
- raw/schoolProfile.json  Detailed profiles, including infrastructure and enrollment (where available).

⚙ Usage
-----
You can use this data in your scripts, apps, or projects. Example (in Node.js):
```js
const schools = require('./raw/schools.json');
console.log(schools[0]);
// Output: { code: "1001", name: "KV AHMEDABAD (SAC)", state_name: "Gujarat", ... }
```

Or open raw/schools.json in your favorite spreadsheet/data tool.

📃 Example Entry
-------------
```JSON
{
  "code": "1001",
  "name": "KV AHMEDABAD (SAC)",
  "state_id": 12,
  "state_name": "Gujarat",
  "region_id": 17,
  "region_name": "AHMEDABAD"
}
```
(raw/schools.json)

📈 Data Updates
------------
- Automated: GitHub Actions update the dataset every 10 days (schools) and every 30 days (profiles).
- Sources: Data fetched from https://pis.kvs.gov.in

👋 Contributing
------------
- Issues and suggestions welcome!
- Data is auto-fetched; PRs for code/scripts or extra documentation are appreciated.

📃 License
-------
This data is under MIT license.

Acknowledgements
----------------
- Kendriya Vidyalaya Sangathan (https://kvsangathan.nic.in/)
- Data fetched from official KVS PIS portal.
