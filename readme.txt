Hangar Ingest — Python 3.11+ standard library and SQLite.
All demonstration measurements are synthetic.
python -m hangar_ingest --db hangar.sqlite3 init
python -m hangar_ingest --db :memory: demo --fixture fixtures/demo.json
python -m hangar_ingest commands
python -m hangar_ingest --db hangar.sqlite3 ingest feed.csv --batch day1 --source feed1 --format csv
python -m hangar_ingest --db hangar.sqlite3 check
python -m unittest discover -s tests -v
python -m compileall -q hangar_ingest
The call command accepts strict JSON operation parameters; commands lists supported operations.
