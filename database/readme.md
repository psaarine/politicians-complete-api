# Database

Database for my politicians app lives here.

## Tables

### Politician

Politician model represents a single politician item. Has relation to the party table.

Columns are:


| Value |Type|explanation|example|
| :--- |:--| :-- | :--|
|first_name|String|politicians name|Maria|
|last_name|String|politicians last name|Ohisalo|
|followers|integer|amount of twitter foollowers| 1421|
|tweets|integer|amount of tweets|1234|
|frequency|integer|frequency of tweets in secs| 3601|
|banner_img| String| link to users profile pic | https/twitter|
|retweets_p|float|Percentage of retweets|0.4|
|e_marks|float|amount of exlamations on a tweet| 3.1|
|q_marks|float|amount of questions on a tweet| 2.5|
|tweet_len|integer|average lenght of a tweet|98|
|likes|integer|average likes to a tweet|152|
|party|foreign|Party abbreviation of a politician|vihr|
<br>
This table is linked via abbreviation to party table

### Party

Serves as a way to group politicians into groups.

|Value|Type|Explanation|Example|
|:---|:---|:---|:---|
|name|String|Name of a party|Vihreät|
|abbreviation|String|abbreviation|Vihr|
|color|String|represents party color| #07fc03|