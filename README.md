# clasp 2.1.0 のテスト

なんか出てたので。
https://developers.google.com/apps-script/guides/clasp

## はじめから TypeScript で書く方法

```sh
npm install -g @google/clasp
clasp login
mkdir clasp_2.1.0_test
cd clasp_2.1.0_test
clasp create clasp_2.1.0_test --rootDir ./src
clasp pull
npm init -y
npm install tslint -D
npm install @types/google-apps-script -S
tslint --init
```

とすると、ローカルに `./src/Code.js` というファイルが配置されるので、コレを `Code.ts` に変更

`.gitignore` に `.clasp.json` と `node_modules/` を追加する

...と、このプロジェクトになります
