## Git Commit Style Guide
ဤ style guide သည် [Udacity Commit Style Guide](https://udacity.github.io/git-styleguide/) ကို မြန်မာလိုကူးယူထားခြင်းဖြစ်သည်။

### Commit Message

#### Message Structure
Commit Message တွေမှာ အပိုင်း၃ပိုင်းပါရမယ်။ 
တခုနဲ့တခုကို blank link တွေနဲ့ခြားထားရမယ်။ 
အပိုင်း၃ပိုင်းက title, optional body နဲ့ optional footer တွေပဲဖြစ်တယ်။
```yaml
type: subject 

body 

footer
```
title မှာဆိုရင် type နဲ့ sybect ပါရမယ်။
type ကတော့ အောက်ပါထဲက တမျိုးဖြစ်နိုင်တယ်။
- **feat**: feature အသစ်ထည့်တဲ့အခါ
- **fix**: bug ကိုပြင်တဲ့အခါ
- **docs**: documentation မှာတခုခုပြင်တဲ့အခါ
- **style**: code ရဲ့အလုပ်လုပ်ပုံကိုမပြောင်းဘဲ tabတွေညှိတာ။ semicolon တွေထည့်တဲ့အခါ။
- **refactor**: production ပုံစံ၀င်အောင် refactor လုပ်တဲ့အခါ
- **test**: test တွေထည့်တဲ့အခါ။ code ကိုမပြောင်းဘဲ testing တွေကို ပြင်တဲ့အခါ။
- **chore**: code ကိုမထိဘဲ package update တင်တာမျိုးတွေ။ config ပြင်တာမျိုးတွေမှာ။
- 
#### Subject
သူကတော့ Capital Letter နဲ့စရေးရမယ်။ စာလုံး၅၀ထက် မပိုရဘူး။ Imperative Tone ပဲသုံးပါ။ တနည်း Verb 1 ပဲသုံးပါ။ Verb 2 မသုံးပါနဲ့။ ဥပမာ။ Changed အစား Change
#### Body
Commit တိုင်းကတော့ body လိုမှာမဟုတ်ဘူး။
အဓိကက commit က ဘာလဲနဲ့ဘာကြောင့်လဲဆိုတာ ရှင်းပြဖို့ပဲ။ ဘယ်လိုလုပ်ထားလဲဆိုတာ ထည့်ရှင်းစရာမလိုဘူး။
Body မှာစာကြောင်းတကြောင်းကို စာလုံး ၇၂လုံးထက်မပိုသင့်။
#### Footer
Footer ကတော့ issue tracker id ကို reference လုပ်ဖို့သုံးပါတယ်။
ဥပမာ။

```markdown
feat: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequenses of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```