# Git & GitHub Collaboration Playground

ဤ repository သည် Code with Thura သင်တန်းသားများအတွက် Git workflow ဖြစ်သည့် **Fork** ပြုလုပ်ခြင်း၊ **Branch** ခွဲခြင်း၊ **Commit** ရေးသားခြင်းနှင့် **Pull Request (PR)** တင်ခြင်းတို့ကို လက်တွေ့ စမ်းသပ်လေ့ကျင့်ရန်အတွက် သီးသန့် ပြုလုပ်ထားသော Sandbox ဖြစ်ပါသည်။

---

## Pull Request တင်ရန် အဆင့်များ

### ၁။ Repository ကို Fork လုပ်ပါ
စာမျက်နှာ၏ ညာဘက်အပေါ်ထောင့်ရှိ **Fork** ခလုတ်ကို နှိပ်ပြီး သင်၏ GitHub အကောင့်ထဲသို့ ကူးယူပါ။

### ၂။ ကွန်ပျူတာထဲသို့ Clone လုပ်ပါ
Terminal သို့မဟုတ် Command Prompt ကိုဖွင့်ပြီး အောက်ပါ command ဖြင့် ဒေါင်းလုဒ်ရယူပါ-
```bash
git clone https://github.com/codewiththura/github-playground.git
cd github-playground

```

### ၃။ Branch အသစ်တစ်ခု ဖွင့်ပါ

`main` branch ပေါ်တွင် တိုက်ရိုက် အလုပ်မလုပ်ဘဲ၊ မိမိကြိုက်နှစ်သက်ရာ အမည်ဖြင့် branch အသစ်တစ်ခု ခွဲထုတ်ပါ-

```bash
git checkout -b test-run/your-filename

```

*(ဥပမာ- `git checkout -b test-run/test-204`)*


### ၄။ ဖိုင်တစ်ခု ဖန်တီးပြီး Commit လုပ်ပါ

1. `sandbox/` folder ထဲသို့ သွားပါ။
2. သင့် branch နာမည်ဖြင့် စမ်းသပ်ဖိုင် အသစ်တစ်ခု ဆောက်ပါ (ဥပမာ- sandbox/test-204.txt)။
3. ထိုဖိုင်ထဲတွင် စာသားများ ရိုက်ထည့်ပါ။ ဥပမာ-
```markdown
Hello Git! Test successful.

```

4. အောက်ပါ command များဖြင့် commit လုပ်ပါ-
```bash
git add .
git commit -m "feat: add test <filename>"

```


### ၅။ GitHub ပေါ်သို့ Push လုပ်ပြီး Pull Request ဖွင့်ပါ

Branch အသစ်ကို GitHub ပေါ်သို့ တင်ပါ-

```bash
git push origin test-run/your-filename

```

ထို့နောက် သင့် GitHub repository စာမျက်နှာသို့သွားပြီး ပေါ်လာသော **Compare & pull request** ခလုတ်ကို နှိပ်ကာ မူရင်း repository သို့ PR ပေးပို့ပါ။

---

## ⚠️ လိုက်နာရန် စည်းကမ်းချက်များ

* အခြားသူများ၏ ဖိုင်များကို ပြင်ဆင်ခြင်း မပြုရပါ။
* ဖိုင်အားလုံးကို `sanbox/` folder ထဲတွင်သာ သီးသန့် အသစ်ဖန်တီး ထည့်သွင်းရပါမည်။
* Branch အမည်၊ Commit message၊ Pull Request ခေါင်းစဉ်/ဖော်ပြချက်နှင့် ဖိုင်တွင်း စာသားများတွင် ကြမ်းတမ်းရိုင်းဆိုင်းသော စကားလုံးများ၊ ဆဲဆိုသရော်မှုများ၊ ခွဲခြားဆက်ဆံသော အသုံးအနှုန်းများနှင့် မဖွယ်မရာ အကြောင်းအရာများ ထည့်သွင်းခြင်းကို လုံးဝ ခွင့်မပြုပါ။
* မူရင်းရှိပြီးသား ဖိုင်များကို ပြင်ဆင်ခြင်း မပြုရပါ။ ဖိုင်အသစ်ကို sandbox/ folder ထဲတွင်သာ သီးသန့် ဆောက်ရပါမည်။
* Pull Request Title ကို `feat: add test <your-filename>` ဟု ရှင်းလင်းစွာ ရေးသားပါ။
