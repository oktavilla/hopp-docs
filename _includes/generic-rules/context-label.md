The Content Item [Category](../data-models/category.md) will always be shown as the first label {% include example-reference.html number="1" %} unless the current one is specifically exempt from being shown in context labels. There may also be additonal labels {% include example-reference.html number="2" %} showing the most relevant tags of the Content Item. Both exemptions and additional labels are defined in the [Product Configuration](../configuration/content-item-context-label-preferences.md).

The platform determines what tags to show in additional labels {% include example-reference.html number="2" %} by looking at:   
A. The list of Tag Groups defined in the Context Label Product Configuration.  
B. Available tags on the Content Item.  
C. The maximum number of labels to show as defined in the Context Label Product Configuration.  

That data will be processed in this order:
1. The platform will look at the first group in (A).
2. We look for tags on the Content Item (B) that belong to that group. 
3. If no tag is matched we try the next group in (A) and try (2) again.
4. If one or more tags match we will show a label.
5. If the maximum number of labels (C) is reached we stop.
6. If we have run though all groups in (A) we stop.
7. We try the next group in (A) and try (2) again.

This will result in 0-(C) additional labels.
