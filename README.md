# ๐ด๊น ๋ช๋ น์ด ์ ๋ฆฌ

#### Branch Remote Local ๊ธฐ๋ณธ ๊ณผ์ 

---

- git init (ํ์ฌ ๋๋ ํ ๋ฆฌ์ git ์ ์ฉ)
- git add README.md (readme ์ถ๊ฐ)
- git commit -m "" (ํ๋์ ๋ฒ์ ์ ํ์คํ ๋ฆฌ์ ์ ์ฅ)
- git status (ํ์ฌ local ์ ์ฉ์ํ ํ์ธ)
- git push (local์ remote๋ก ์ ์ฅ)
- git pull (remote๋ฅผ local๋ก ์ ์ฅ)

#### Branch ๋ช๋ น์ด ( Local Repository )
---
- git branch (๋ก์ปฌ ๋ธ๋์น ๋ชฉ๋ก ์กฐํ)
- git branch -r (์๊ฒฉ ๋ธ๋์น ๋ชฉ๋ก ์กฐํ)
- git branch -a (๋ชจ๋  ๋ธ๋์น ๋ชฉ๋ก ์กฐํ)
- git branch {๋ธ๋์น๋ช} ( local ๋ธ๋์น ์์ฑ)
- git checkout -b {๋ธ๋์น๋ช} (๋ช๋ น์ด๋ฅผ ํตํด ์ ๊ท ๋ธ๋์น ์์ฑ๊ณผ ๋์์ ์ฒดํฌ์์)
- git checkout {๋ธ๋์น๋ช} (๋ธ๋์น ๋ณ๊ฒฝ)
- git branch -d {๋ธ๋์น๋ช} ( ๋ธ๋์น ์ญ์  )

#### ์๊ฒฉ ์ ์ฅ์( remote repository )

---

- git push origin -u <new_name_branch> (Remote Branch(์๊ฒฉ ๋ธ๋์น) ์ด๋ฆ ๋ณ๊ฒฝ ๋ฐฉ๋ฒ)
- git remote -v (ํ์ฌ ์ฐ๊ฒฐ๋์ด ์๋ ์๊ฒฉ ๋ ํ์งํ ๋ฆฌ๋ฅผ ํ์ธ)
- git remote add <name> <url> (์๊ฒฉ์ ์ฅ์์ ์ฐ๊ฒฐํ๊ณ  ์ถ์ผ์ค ๊ฒฝ์ฐ์)
- git clone [์ ์ฅ์ ์ฃผ์] ( ์ ์ฅ์ ๋ณต์  )
- git fetch (remote๋ฅผ local๋ก ์ ์ฅ, ์ง์  ๋น๊ต๋์กฐ ํ์ ์๋ merge)
- git pull (remote๋ฅผ local๋ก ์ ์ฅ, ์๋ merge)
  
#### (โยดโก`โ)๋ก์ปฌ์ด๋ ์๊ฒฉ ๋ธ๋์น ์ญ์ ํ๊ธฐ
---
###### ๋ก์ปฌ๋ธ๋ ์น ์ ๊ฑฐ
- git branch -d <branch_name>
###### ์๊ฒฉ๋ธ๋ ์น ์ ๊ฑฐ
- git push origin --delete feature/TEST-860
- git branch -d TEST (๋ก์ปฌ์ ๊ฑฐ)
    + git push origin TEST (์๊ฒฉ๋ฐ์)

#### merge
---
- git merge <๋ค๋ฅธ branch์ด๋ฆ>   ํ์ฌ branch์ ๋ค๋ฅธ branch์ ์์ ์ฌํญ ํฉ์น๊ธฐ
- git diff <branch์ด๋ฆ>    ๋ณ๊ฒฝ ๋ด์ฉ์ ํฉ์ฐจ๊ธฐ์ ์ ๋ฐ๋ ๋ด์ฉ์ ๋น๊ตํ  ์ ์๋ค. 
                                              
# ๐ ๊น ๊ธฐ๋ณธ์ฌ์ฉ
#### 1. ๋๋ ํ ๋ฆฌ ๋ค์ด๊ฐ๊ธฐ

###### git bash
- $ cd "C:\Users\gittest\Desktop\git_practice"  <- " "๋ฅผ ๋ถ์ฌ์ค์ผํ๋ค.                                                 
                                                 
                                                 
#### 2. ์ฌ์ฉ์๋ฑ๋ก

- git config --global user.email "[์ด๋ฉ์ผ์ฃผ์]"
- git config --global user.name "[์ด๋ฉ์ผ์ฃผ์]"                                                 
#### 3. ์ ์ฅ์์์ฑ

- git init
  + master branch ์์ฑ, git bash ํด๋๋ช์ (master)์ถ๊ฐ๋, .git์ด๋ผ๋ ์จ๊นํด๋ ์ถ๊ฐ                                       
#### 4. ์คํ์ด์ง์ ์ฌ๋ฆฌ๊ธฐ

- git add .(์ ์ฒดํด๋ >> ํน์ ํด๋๋ช ์ง์ ๊ฐ๋ฅ)
- git status
#### 5. ๋ก์ปฌ์ ์ธ์ด๋ธ

- git commit -m "์ปค๋ฐ๋ฉ์ธ์ง"
- git log 
  + commit๋ ๋ฆฌ์คํธ๋ฅผ ๋ณด์ฌ์ค
#### 6. ์๊ฒฉ์ ์ฅ์ ์ฐ๋

- git remote add origin https://github.com/myungyi0314/githubTest.git
- git remote -v
#### 7. ์๊ฒฉ์ ์ฅ์์ ์ฌ๋ฆฌ๊ธฐ

- git push origin master 

# ๐ข๊น fork์ clone ๋น๊ต
#### fork
---
#### clone
---
๐ด๐ ๐ก๐ข๐ต๐ฃ๐คโซโช                                                 
# ๋งํฌ์ ์ธ์ด markup
- ํ๊ทธ ๋ฑ์ ์ด์ฉํ์ฌ ๋ฌธ์๋ ๋ฐ์ดํฐ์ ๊ตฌ์กฐ๋ฅผ ๋ช์ํ๋ ์ธ์ด
- html
# ๋งํฌ๋ค์ด ์ธ์ด markdown
- ์ผ๋ฐ ํ์คํธ ๊ธฐ๋ฐ์ ๊ฒฝ๋ ๋งํฌ์ ์ธ์ด
- .md๋ผ๋ ํ์ฅ์๋ฅผ ์ฌ์ฉ
- github์ wiki๋ readme
- notion, slack                                                   

#### ๋งํฌ๋ค์ด ์ฌ์ฉ๋ฒ
```
# Hello, github
## Hello, github
### Hello, github
#### Hello, github
##### Hello, github
###### Hello, github
```
  
