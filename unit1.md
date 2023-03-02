---
layout: page
title: "Unit 1 - An Introduction to Python Programming and the OO Programming Paradigm"
permalink: /unit1/
---

## Article Review
- Review the article by Di Silvestro & Nadir (2021). Discuss one aspect of this article which you find unexpected.
- Di Silvestro, F., & Nadir, M. (2021). The Power of ePortfolio Development to Foster Reflective and Deeper Learning in an Online Graduate Adult Education Program. Adult Learning, 32(4), 154-164. https://doi.org/10.1177/1045159520977735

---
{: data-content="Discussion"}

In their article, Di Silvestro and Nadir (2021) investigate the effects of ePortfolio development on reflective and deeper learning in an online graduate adult education program. One aspect of the article that I found unexpected was the finding that ePortfolios can help foster a sense of community among online learners. The authors suggest that through the use of ePortfolios, students were able to share their learning experiences with their peers, receive feedback and support, and build relationships with other learners. This finding is in line with previous research that suggests that ePortfolios can help build a sense of community among online learners (Kumar & Rose, 2017; Puzziferro, 2008).

Moreover, the authors point out that ePortfolios can be used to assess students' learning outcomes and achievements. They note that ePortfolios provide a comprehensive and holistic picture of students' learning, which can be used to evaluate the effectiveness of the online education program. This finding is supported by previous research that indicates ePortfolios can be used for both formative and summative assessments (Lorenzo & Ittelson, 2005; Jafari et al., 2006).

Overall, this article highlights the potential of ePortfolio development to enhance students' learning experiences in online graduate adult education programs, and underscores the importance of reflective and deeper learning in achieving meaningful learning outcomes.

<b>References</b>:
Di Silvestro, F., & Nadir, M. (2021). The Power of ePortfolio Development to Foster Reflective and Deeper Learning in an Online Graduate Adult Education Program. Adult Learning, 32(4), 154-164.

Jafari, A., Laffey, J., & Lopez-Fernandez, O. (2006). Toward effective evaluation and reform in ePortfolios. Educause Quarterly, 29(2), 28-35.

Kumar, S., & Rose, G. (2017). Building a community of learners through ePortfolios. Journal of Education and Practice, 8(15), 59-66.

Lorenzo, G., & Ittelson, J. (2005). An overview of e-portfolios. Educause Learning Initiative, 1(2005), 1-27.

Puzziferro, M. (2008). Online technologies self-efficacy and self-regulated learning as predictors of final grade and satisfaction in college-level online courses. American Journal of Distance Education, 22(2), 72-89.

---

## Develop a Python program and apply protected and unprotected variables within it.

```py	
# Protected and unprotected variables
class gmailAccount():
  """An example class to represent the data fields you would need to login to an email account.
  The email and password variables are protected and unprotected variables, respectively 
  """
  def __init__(self, email, password):
    self.email = email # unprotected variable
    self._password = password # protected variable

# Create an instance of the gmailAccount class 
myAccount = gmailAccount("Nkosi", "1234")
# Print the email and password variables
print(myAccount.email)
print(myAccount._password)
```
