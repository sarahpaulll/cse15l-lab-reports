# Lab Report 3

## grep ^character
The command grep ^character matches the given character at the beginning of the line in the file or directory it is searching in. This command is useful because it will display the lines that start with the given character. 
```
# Example One: Input
grep ^J written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt 

```
```
# Example One: Output 
Jacques Cousteau made El Garrafón famous in the 1960s, when he filmed the nurse sharks in their caves in the park. You can still find them at the Cave of the Sleeping Sharks, and experienced divers can swim with them — not as frightening as you would think, as nurse sharks are not dangerous to humans — in their dark, watery hideouts. Non-certified divers who want the chance can swim with the sharks at El Garrafón pier, where several sharks are kept in pens for this purpose. The marine life is truly spectacular at the park, both in the shallow and the outer reef areas. The land around the southern tip of the island is also protected; Punta Sur is a wind-swept, salty spot where the waves of the Caribbean crash onto the rocks. The remains of a Mayan temple can be seen here, along with a lighthouse that guides sailors safely to port to this day.
Just south of Puerto Aventuras is Xel-Ha, a network of mangrove, waterways, pools, and caves that was once a Mayan site. The majority of the remains form an archaeological site on the inland side of the main highway; Xel-Ha Park sits on the seaward side. This park has more natural areas than Xcaret for snorkeling and exploring, but fewer organized activities, though there is a “swim with the dolphins” program. At either side of this managed park are public inlets; at Akumal you can snorkel just off the sand, or rent a boat to take you out to the reef.
```
```
# Example Two: Input
grep ^Z written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt

```
```
# Example Two: Output
Zaanse Schans
Zaanse Schans is the archetypal Dutch landscape personified, and lies just a few miles north of Amsterdam center in the suburb of Zaadam.

```


## grep -r
The command grep -r will search for a string in the currect directory and all subdirectories
```
# Example One: Input
grep -r "Zaanse" *
```
```
# Example One: Output
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:Zaanse Schans
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:Zaanse Schans is the archetypal Dutch landscape personified, and lies just a few miles north of Amsterdam center in the suburb of Zaadam.
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:This landscape is no accident or happy coincidence but a living museum created in 1960, which has brought together a number of farmhouses, windmills, dairies, and barns — real agricultural buildings which would have been demolished had they not been relocated here. Zaanse Schans has working mills, cheese-making factories, and clog workshops, situated on a canalside. You are free to explore at your own pace and maybe enjoy a pannekoeken (pancake) while you’re there.
```
```
# Example Two: Input
grep -r "Bob and Sharon" *
```
```
# Example Two: Output
written_2/non-fiction/OUP/Berk/ch1.txt:•Bob and Sharon, parents of a 4-year-old: Our daughter, Lydia, could recite her ABCs and count from 1 to 20 by age 2 1/2. When we looked for a preschool, many programs appeared to do little more than let children play, so we chose one with lots of emphasis on academics. To me, Lydia’s preschool seems like great preparation for kindergarten and ﬁrst grade, but each morning, Lydia hates to go. Why is Lydia, who’s always been an upbeat, curious child, so unhappy?
```

## grep -i

## grep -n
