# Privacy of MarqueTaPage Desktop

**In short: your documents never leave your computer.** No account, no cloud, no telemetry, no advertising, no
automatic update.

## What the software sends over the Internet

Nothing. At startup, the software cuts all network access inside its own program: even by mistake, it could not send
anything. Its source code is visible so that anyone can check this.

Two actions open another program, only when you click: the contact address (your email program) and, where relevant, a
web page (your browser).

## Updates: only if you ask

The software never checks by itself whether a newer version exists. If you choose Help > Check for updates and answer
"Yes" to the message shown, it connects to GitHub (api.github.com), and to nothing else, to read the number of the
latest published version. It sends the name and version of the software, like any request to a website; GitHub sees
your IP address. No document, name, recipient or history is sent. The connection is open for the time of this check,
then closed again.

## Word, OpenDocument and text files

For these files, the software asks Microsoft Word or LibreOffice, if installed on your computer, to convert them to
PDF. This conversion happens on your computer. Word and LibreOffice are separate programs with their own settings:
depending on these, they may for instance load an image linked in a document from the Internet. PDFs and photos use
neither Word nor LibreOffice.

## What is stored on your computer

| File | Content | How to delete it |
|---|---|---|
| `.filigrane_mes_documents.json` (home folder) | appearance settings: color, opacity, size, theme | delete the file |
| `.filigrane_mes_documents_historique.json` (home folder) | history: date, recipient, purpose and location of the copies | "Clear history" button in the pane, or delete the file |

The watermark text is never saved in the settings. On Linux, the history is readable only by you. The temporary files
of a conversion are deleted as soon as it is finished.

## Watermarked copies

The watermark is part of the image: it cannot be removed like a layer. The hidden information of the original file
(GPS position of a photo, device, author, title) is removed. The copy carries neither the publisher's name nor the
software's. Its suggested name is that of the original followed by `_filigrane`: you can change it when saving.

A watermark makes fraudulent reuse of a copy harder and more visible; it cannot prevent it in every case. Keep your
originals.

## Contact

Anthony BELKACEM EI, 200 rue de la Croix Nivert, 75015 Paris, France. Questions: apps@ohtna.fr
