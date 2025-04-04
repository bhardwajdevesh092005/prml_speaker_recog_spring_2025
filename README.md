# prml_speaker_recog_spring_2025
If you encounter the error:
```sh
'vite' is not recognized as an internal or external command
```
Follow these steps to resolve it:

1.Ensure dependencies are installed
Run the following command in the project root:
```sh
npm install
```

2.Manually install Vite (if needed)
```sh
npm install vite --save-dev
```

3.Verify the `package.json` script section contains:
```json
"scripts": {
"dev": "vite",
"build": "vite build",
"serve": "vite preview"
}
```

4.Delete `node_modules` and reinstall dependencies (if issues persist)
```sh
rm -rf node_modules package-lock.json
npm install
npm run dev
```
(For Windows PowerShell: use `Remove-Item -Recurse -Force node_modules, package-lock.json` instead of `rm -rf`.)

### Installing Librosa  

5. Librosa can be installed using pip with the following command:  
```bash
pip install librosa
#Ensure you have the necessary dependencies by running:

pip install numpy scipy joblib soundfile audioread  