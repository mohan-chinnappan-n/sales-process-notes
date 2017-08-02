## Controlling access to the Opportunity based on particular Opportunity.Stage to non-owner users

#### Use case: Company: ACME computing
- Org-wide-default of Opportunity is *private*
- Likes to introduce new Opportunity Stage called: **Discontinued**
- Likes to provide read-only access to the Opportunities ( to the non-owners) with a restriction: they can see the Opportunities that they do not own while the Opportunity Stage is NOT **Discontinued**

#### Steps	

- Make sure Org-wide-default for Opportunity is private

![Owd oppty is private](./img/owd-oppty-private.png) 

- Create new item for Opportunity.Stage **Discontinued** with Probability 0%

![Add new Opportunity stage ](./img/adding-oppty-stage-discontinued.png) 

- User Joe Simple *can* see the **Discontinued** Opportunities now:

![Joe can see Discontinued Opportunities  ](./img/joe-can-see-discontined-opptys.png) 

- Create a criteria based sharing rule for Opportunity to:  provide read-only access to the Opportunities (to non-owners) with a restriction: they can see the Opportunities they do not own while Opportunity Stage is NOT **Discontinued**

![criteria based sharing rule for Opportunity](./img/criteria-based-sharing-rule.png) 

- Now user Joe Simple *can't* see **Discontinued** Opportunities:
 ![Joe can't see Discontinued Opportunities  ](./img/joe-cant-see-discontinued-oppty.png) 




