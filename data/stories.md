## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

<!---------- Affirmative Action ---------->
## start path
* greet
  - utter_greet
  - utter_opening
  - utter_openning_Q
* agree OR disagree
  - utter_affir_act_intro
  - utter_pos_discri_Q
> check_pos_discri_Q

## agree with "postive discrimination"
> check_pos_discri_Q
* agree 
  - utter_born_equal_Q
> check_born_equal_Q

## disagree with "postive discrimination"
> check_pos_discri_Q
* disagree
  - utter_event_cause_Q
> check_event_cause_Q

## agree with born equal
> check_born_equal_Q
* agree 
  - utter_NBA_Q
* agree OR disagree
  - utter_individuality_Q
* agree OR disagree
  - utter_balance
* agree OR disagree
  - utter_judge_someone_Q
> check_judge_someone_Q

## disagree with born equal
> check_born_equal_Q
* disagree
  - utter_such_world_Q
> check_such_world_Q

## agree with such world
> check_such_world_Q
* agree 
  - utter_individuality_Q
* agree OR disagree
  - utter_balance
* agree OR disagree
  - utter_judge_someone_Q
> check_judge_someone_Q

## disagree with such world
> check_such_world_Q
* disagree
  - utter_balance
* agree OR disagree
  - utter_judge_someone_Q
> check_judge_someone_Q

## agree with judge someone
> check_judge_someone_Q
* agree 
  - utter_those_people_Q
> check_those_people_Q

## disagree with judge someone
> check_judge_someone_Q
* disagree
  - utter_statistically_Q
> check_statistically_Q

## choose one among those people
> check_those_people_Q
* choose_one
  - utter_race_gender

## not choose one among those people
> check_those_people_Q
* not_choose_one
  - utter_statistically_Q
> check_statistically_Q

## agree with statistically
> check_statistically_Q
* agree 
  - utter_target_Q
> check_target_Q

## disagree with statistically
> check_statistically_Q
* disagree
  - utter_race_gender

## agree with target
> check_target_Q
* agree 
  - utter_who_decides_Q
* agree OR disagree
  - utter_race_gender

## disagree with target
> check_target_Q
* disagree
  - utter_race_gender

## agree with event and cause
> check_event_cause_Q
* agree 
  - utter_lasting_effect_Q
> check_lasting_effect_Q

## disagree with event and cause
> check_event_cause_Q
* disagree
  - utter_common_Q
> check_common_Q

## agree with common
> check_common_Q
* agree 
  - utter_lasting_effect_Q
> check_lasting_effect_Q

## disagree with common
> check_common_Q
* disagree
  - utter_card_game_Q
* agree OR disagree
  - utter_only_fair
* agree OR disagree
  - utter_hardship_counts_Q
> check_hardship_counts_Q

## agree with lasting effect
> check_lasting_effect_Q
* agree 
  - utter_card_game_Q
* agree OR disagree
  - utter_only_fair
* agree OR disagree
  - utter_hardship_counts_Q
> check_hardship_counts_Q

## disagree with lasting effect
> check_lasting_effect_Q
* disagree
  - utter_only_fair
* agree OR disagree
  - utter_hardship_counts_Q
> check_hardship_counts_Q

## agree with hardship counts
> check_hardship_counts_Q
* agree 
  - utter_work_harder_Q
> check_work_harder_Q

## disagree with hardship counts
> check_hardship_counts_Q
* disagree
  - utter_tennis_comp_Q
* answer_tennis_comp
  - utter_provide_opportunities
* agree OR disagree
  - utter_closing
  - utter_goodbye

## agree with work harder
> check_work_harder_Q
* agree
  - utter_provide_opportunities
* agree OR disagree
  - utter_closing
  - utter_goodbye

## disagree with work harder
> check_work_harder_Q
* disagree
  - utter_most_people_Q
* agree OR disagree
  - utter_provide_opportunities
* agree OR disagree
  - utter_closing
  - utter_goodbye

<!---------- Gun Laws ---------->

<!---------- Abortion / Pro-Life Movement ---------->

<!---------- Vaccination ---------->