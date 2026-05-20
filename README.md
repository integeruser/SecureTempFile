# SecureTempFile

SecureTempFile is a small browser-based wrapper around [TempFile.org](https://tempfile.org) for secure temporary file sharing.

The wrapper encrypts the selected file locally in the browser, then stores only the encrypted copy on TempFile.org (but with the original filename).

After encryption and upload, the wrapper generates a shareable download link. When someone opens the link, the encrypted file is downloaded from TempFile.org and automatically decrypted directly in their browser before being saved locally. The passphrase for decryption is stored in the URL hash fragment (which is never transmitted to the server).

TempFile.org will auto-delete the uploaded file after 24 hours.
