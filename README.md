# DA_Assingment8.1

Ans1
td1 <- td %>%
   filter(smoking == "Nonsmoker") %>%
  summarize(average = mean(salary))

td1

td2 <- td %>%
   filter(smoking == "Smoker") %>%
  summarize(average = mean(salary))

tdg1 <- td %>%
  filter(gender == "Male") %>%
  summarize(gender= 'Male', average = mean(salary))

tdg1

tdg2 <- td %>%
  filter(gender == "Female") %>%
  summarize(gender= 'Female', average = mean(salary))

tdg2

-- Male gender has the highest mean salary gender  average
1   Male 743.3915
-- 
--724.5164 is the highest mean salary

---> sdg2 <- td %>%
+   filter(gender == "Female") %>%
+   summarize(gender= 'Female', sd = sd(salary))
> sdg2
  gender       sd
1 Female 130.7053

> sdg1 <- td %>%
+   filter(gender == "Male") %>%
+   summarize(gender= 'Male', sd = sd(salary))
> sdg1
  gender       sd
1   Male 158.5423
