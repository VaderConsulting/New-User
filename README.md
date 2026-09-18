# New User

Chips, Bits and Bytes VB6 domain user provisioning UI (form `frmMain` caption "Add User"). Loads WinNT domain groups via ADSI (`IADsDomain`) and siteloc rows from a SQL Server POLICE catalog over ADO, then fills home directory and profile paths from the chosen siteserver. Collects username, fullname, logon script, duty option (OIC / Detective / General), and dual-list group membership for the WARNBRO domain; OK/Check handlers are not present in this working copy.

**Source last updated:** 2026-08-27 · **Language:** VB6 · **Target:** VB6 Win32 · **Output:** WinForms exe

_Note: original OneDrive LastWriteTime values were wiped to 2026-08-27 by a zip transfer; date above uses best available evidence (headers/copyright where helpful)._

## Solution structure

| Project | Language | Type | Purpose |
|---------|----------|------|---------|
| `Project1` (`New User.vbp`) | VB6 | WinForms exe | ADSI/ADO Add User form for domain account fields and group picks |

## How to open

Open the `.vbp` in Visual Basic 6.0 IDE:
- `New User.vbp`

## Requirements

- Visual Basic 6.0 IDE
- Microsoft ActiveX Data Objects 2.5 and Active DS Type Library
- Reachable SQL Server DSN (`POLICE` catalog) and WinNT domain (default WARNBRO) matching the Form_Load connection string

## Attribution and provenance

Working copy from Dave Robinson's OneDrive Historical Dev folder `VB/Old/New User`.
Company names in project files: Chips, Bits and Bytes.

## License

MIT (c) 2026 VaderConsulting for Dave Robinson's code. See `LICENSE`.
