## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

<!---------- Affirmative Action ---------->
## start path - Affirmative Action
* aff_action_greet OR greet
  - utter_greet
  - utter_opening
  - utter_openning_Q
* agree OR disagree
  - utter_aff_act_intro
  - utter_pos_discri_Q
> check_pos_discri_Q

## agree with "postive discrimination" - Affirmative Action
> check_pos_discri_Q
* agree 
  - utter_born_equal_Q
> check_born_equal_Q

## disagree with "postive discrimination" - Affirmative Action
> check_pos_discri_Q
* disagree
  - utter_event_cause_Q
> check_event_cause_Q

## agree with born equal - Affirmative Action
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

## disagree with born equal - Affirmative Action
> check_born_equal_Q
* disagree
  - utter_such_world_Q
> check_such_world_Q

## agree with such world - Affirmative Action
> check_such_world_Q
* agree 
  - utter_individuality_Q
* agree OR disagree
  - utter_balance
* agree OR disagree
  - utter_judge_someone_Q
> check_judge_someone_Q

## disagree with such world - Affirmative Action
> check_such_world_Q
* disagree
  - utter_balance
* agree OR disagree
  - utter_judge_someone_Q
> check_judge_someone_Q

## agree with judge someone - Affirmative Action
> check_judge_someone_Q
* agree 
  - utter_those_people_Q
> check_those_people_Q

## disagree with judge someone - Affirmative Action
> check_judge_someone_Q
* disagree
  - utter_statistically_Q
> check_statistically_Q

## choose one among those people - Affirmative Action
> check_those_people_Q
* choose_one
  - utter_race_gender
* agree OR disagree
  - utter_closing
  - utter_goodbye

## not choose one among those people - Affirmative Action
> check_those_people_Q
* not_choose_one
  - utter_statistically_Q
> check_statistically_Q

## agree with statistically - Affirmative Action
> check_statistically_Q
* agree 
  - utter_target_Q
> check_target_Q

## disagree with statistically - Affirmative Action
> check_statistically_Q
* disagree
  - utter_race_gender
* agree OR disagree
  - utter_closing
  - utter_goodbye

## agree with target - Affirmative Action
> check_target_Q
* agree 
  - utter_who_decides_Q
* agree OR disagree
  - utter_race_gender
* agree OR disagree
  - utter_closing
  - utter_goodbye

## disagree with target - Affirmative Action
> check_target_Q
* disagree
  - utter_race_gender
* agree OR disagree
  - utter_closing
  - utter_goodbye

## agree with event and cause - Affirmative Action
> check_event_cause_Q
* agree 
  - utter_lasting_effect_Q
> check_lasting_effect_Q

## disagree with event and cause - Affirmative Action
> check_event_cause_Q
* disagree
  - utter_common_Q
> check_common_Q

## agree with common - Affirmative Action
> check_common_Q
* agree 
  - utter_lasting_effect_Q
> check_lasting_effect_Q

## disagree with common - Affirmative Action
> check_common_Q
* disagree
  - utter_card_game_Q
* agree OR disagree
  - utter_only_fair
* agree OR disagree
  - utter_hardship_counts_Q
> check_hardship_counts_Q

## agree with lasting effect - Affirmative Action
> check_lasting_effect_Q
* agree 
  - utter_card_game_Q
* agree OR disagree
  - utter_only_fair
* agree OR disagree
  - utter_hardship_counts_Q
> check_hardship_counts_Q

## disagree with lasting effect - Affirmative Action
> check_lasting_effect_Q
* disagree
  - utter_only_fair
* agree OR disagree
  - utter_hardship_counts_Q
> check_hardship_counts_Q

## agree with hardship counts - Affirmative Action
> check_hardship_counts_Q
* agree 
  - utter_work_harder_Q
> check_work_harder_Q

## disagree with hardship counts - Affirmative Action
> check_hardship_counts_Q
* disagree
  - utter_tennis_comp_Q
* answer_tennis_comp
  - utter_provide_opportunities
* agree OR disagree
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## agree with work harder - Affirmative Action
> check_work_harder_Q
* agree
  - utter_provide_opportunities
* agree OR disagree
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## disagree with work harder - Affirmative Action
> check_work_harder_Q
* disagree
  - utter_most_people_Q
* agree OR disagree
  - utter_provide_opportunities
* agree OR disagree
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

<!---------- Free Speech ---------->
## start path - Free Speech
* free_speech_greet
  - utter_greet
  - utter_opening
  - utter_openning_Q
* agree OR disagree
  - utter_free_speech_intro
  - utter_free_speech_believe_Q
> check_free_speech_believe_Q

## believe with "free speech" - Free Speech
> check_free_speech_believe_Q
* agree 
  - utter_imagine_situation_Q
> check_imagine_situation_Q

## agree with "imagine situation" - Free Speech
> check_imagine_situation_Q
* agree 
  - utter_rumour_protect_Q
* agree OR disagree
  - utter_abusive_speech_Q
* agree OR disagree
  - utter_safe_happy_Q
* agree OR disagree
  - utter_by_majority_Q
> check_by_majority_Q

## disagree with "imagine situation" - Free Speech
> check_imagine_situation_Q
* disagree 
  - utter_perfectly_comfortable_Q
* agree OR disagree
  - utter_abusive_speech_Q
* agree OR disagree
  - utter_safe_happy_Q
* agree OR disagree
  - utter_by_majority_Q
> check_by_majority_Q

## agree with "by majority" - Free Speech
> check_by_majority_Q
* agree
  - utter_flat_earth_Q
* agree OR disagree
  - utter_informed_decision_Q
> check_informed_decision_Q

## disagree with "by majority" - Free Speech
> check_by_majority_Q
* disagree
  - utter_informed_decision_Q
> check_informed_decision_Q

## agree with "informed decision" - Free Speech
> check_informed_decision_Q
* agree
  - utter_restrict_misinfo_Q
* agree OR disagree
  - utter_spreads_fast_Q
* agree OR disagree
  - utter_closing
  - utter_goodbye

## disagree with "informed decision" - Free Speech
> check_informed_decision_Q
* disagree
  - utter_climate_catastrophe_Q
* agree OR disagree
  - utter_spreads_fast_Q
* agree OR disagree
  - utter_closing
  - utter_goodbye

## not believe with "free speech" - Free Speech
> check_free_speech_believe_Q
* disagree 
  - utter_20_years_Q
> check_utter_20_years_Q

## agree with "20 years" - Free Speech
> check_utter_20_years_Q
* agree
  - utter_no_vote_Q
* agree OR disagree
  - utter_free_discuss_Q
> check_free_discuss_Q

## agree with "20 years" - Free Speech
> check_utter_20_years_Q
* disagree
  - utter_free_discuss_Q
> check_free_discuss_Q

## agree with "free discuss" - Free Speech
> check_free_discuss_Q
* agree
  - utter_challenge_freely_Q
* agree OR disagree
  - utter_who_restricts_Q
* agree OR disagree
  - utter_how_right_Q
* agree OR disagree
  - utter_censor_certain_Q
> check_censor_certain_Q

## disagree with "free discuss" - Free Speech
> check_free_discuss_Q
* disagree
  - utter_new_ideas_Q
* agree OR disagree
  - utter_who_restricts_Q
* agree OR disagree
  - utter_how_right_Q
* agree OR disagree
  - utter_censor_certain_Q
> check_censor_certain_Q

## agree with "censor certain" - Free Speech
> check_censor_certain_Q
* agree
  - utter_horrendous_Q
* agree OR disagree
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## disgree with "censor certain" - Free Speech
> check_censor_certain_Q
* disagree
  - utter_totalitarian_Q
> check_totalitarian_Q

## agree with "totalitarian" - Free Speech
> check_totalitarian_Q
* agree
  - utter_ideas_silenced_Q
* agree OR disagree
  - utter_horrendous_Q
* agree OR disagree
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## disagree with "totalitarian" - Free Speech
> check_totalitarian_Q
* disagree
  - utter_horrendous_Q
* agree OR disagree
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

<!---------- Gun Laws ---------->

<!---------- Abortion / Pro-Life Movement ---------->

<!---------- Vaccination ---------->