## say goodbye
* goodbye
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## bot challenge
* bot_challenge
  - utter_iamabot

<!-------------------------------------------------------------------------->
<!--------------------------- Affirmative Action --------------------------->
<!-------------------------------------------------------------------------->

## start path - Affirmative Action
* aff_action_greet OR greet
  - utter_greet
  - utter_opening
  - utter_openning_Q
> check_aff_openning_Q

<!---------- Question: openning question ---------->
# Agree or disagree with openning questions - Affirmative Action
> check_aff_openning_Q
* agree OR disagree 
  - utter_aff_act_intro
  - utter_pos_discri_Q
> check_pos_discri_Q

# Can not understand the respond to openning questions - Affirmative Action
> check_aff_openning_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_aff_openning_Q

<!---------- Question: postive discrimination ---------->
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

## Can not understand "postive discrimination" - Affirmative Action
> check_pos_discri_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_pos_discri_Q

<!---------- Question: born equal ---------->
## agree with born equal - Affirmative Action
> check_born_equal_Q
* agree
  - utter_NBA_Q
> check_NBA_Q

## disagree with born equal - Affirmative Action
> check_born_equal_Q
* disagree
  - utter_such_world_Q
> check_such_world_Q

## Can not understand born equal - Affirmative Action
> check_born_equal_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_born_equal_Q

<!---------- Question: NBA ---------->
## agree or disagree with NBA - Affirmative Action
> check_NBA_Q
* agree OR disagree
  - utter_individuality_Q
> check_individuality_Q

## Can not understand NBA - Affirmative Action
> check_NBA_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_NBA_Q

<!---------- Question: individuality ---------->
## agree or disagree with individuality - Affirmative Action
> check_individuality_Q
* agree OR disagree
  - utter_balance
> check_utter_balance

## Can not understand individuality - Affirmative Action
> check_individuality_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_individuality_Q

<!---------- Question: balance ---------->
## agree or disagree with balance - Affirmative Action
> check_utter_balance
* agree OR disagree
  - utter_judge_someone_Q
> check_judge_someone_Q

## Can not understand balance - Affirmative Action
> check_utter_balance
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_utter_balance

<!---------- Question: such world ---------->
## agree with such world - Affirmative Action
> check_such_world_Q
* agree 
  - utter_individuality_Q
> check_individuality_Q

## disagree with such world - Affirmative Action
> check_such_world_Q
* disagree
  - utter_balance
> check_utter_balance

## Can not understand such world  - Affirmative Action
> check_such_world_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_such_world_Q

<!---------- Question: judge someone ---------->
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

## Can not understand judge someone - Affirmative Action
> check_judge_someone_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_judge_someone_Q

<!---------- Question: choose those people ---------->
## choose one among those people - Affirmative Action
> check_those_people_Q
* choose_one OR agree
  - utter_race_gender
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## not choose one among those people - Affirmative Action
> check_those_people_Q
* not_choose_one OR disagree
  - utter_statistically_Q
> check_statistically_Q

## Can not understand choose those people - Affirmative Action
> check_those_people_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_those_people_Q

<!---------- Question: statistically ---------->
## agree with statistically - Affirmative Action
> check_statistically_Q
* agree 
  - utter_target_Q
> check_target_Q

## disagree with statistically - Affirmative Action
> check_statistically_Q
* disagree
  - utter_race_gender
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand statistically - Affirmative Action
> check_statistically_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_statistically_Q

<!---------- Question: target ---------->
## agree with target - Affirmative Action
> check_target_Q
* agree 
  - utter_who_decides_Q
> check_who_decides_Q

## disagree with target - Affirmative Action
> check_target_Q
* disagree
  - utter_race_gender
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand target - Affirmative Action
> check_target_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_target_Q

<!---------- Question: who decides ---------->
## agree or disagree with who decides - Affirmative Action
> check_who_decides_Q
* agree OR disagree
  - utter_race_gender
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand who decides - Affirmative Action
> check_who_decides_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_who_decides_Q

<!---------- Question: event and cause ---------->
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

## Can not understand who decides - Affirmative Action
> check_event_cause_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_event_cause_Q

<!---------- Question: common ---------->
## agree with common - Affirmative Action
> check_common_Q
* agree 
  - utter_lasting_effect_Q
> check_lasting_effect_Q

## disagree with common - Affirmative Action
> check_common_Q
* disagree
  - utter_card_game_Q
> check_card_game_Q

## Can not understand common - Affirmative Action
> check_common_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_common_Q

<!---------- Question: card game ---------->
## agree or disagree with card game - Affirmative Action
> check_card_game_Q
* agree OR disagree
  - utter_only_fair
> check_only_fair

## Can not understand card game - Affirmative Action
> check_card_game_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_card_game_Q

<!---------- Question: only fair ---------->
## agree or disagree with only fair - Affirmative Action
> check_only_fair
* agree OR disagree
  - utter_hardship_counts_Q
> check_hardship_counts_Q

## Can not understand only fair - Affirmative Action
> check_only_fair
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_only_fair

<!---------- Question: lasting effect ---------->
## agree with lasting effect - Affirmative Action
> check_lasting_effect_Q
* agree 
  - utter_card_game_Q
> check_card_game_Q

## disagree with lasting effect - Affirmative Action
> check_lasting_effect_Q
* disagree
  - utter_only_fair
> check_only_fair

## Can not understand lasting effect - Affirmative Action
> check_lasting_effect_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_lasting_effect_Q

<!---------- Question: hardship counts ---------->
## agree with hardship counts - Affirmative Action
> check_hardship_counts_Q
* agree 
  - utter_work_harder_Q
> check_work_harder_Q

## disagree with hardship counts - Affirmative Action
> check_hardship_counts_Q
* disagree
  - utter_tennis_comp_Q
> check_tennis_comp_Q

## Can not understand hardship counts - Affirmative Action
> check_hardship_counts_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_hardship_counts_Q

<!---------- Question: tennis comp ---------->
## answer tennis comp - Affirmative Action
> check_tennis_comp_Q
* answer_tennis_comp
  - utter_provide_opportunities
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand tennis comp - Affirmative Action
> check_tennis_comp_Q
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR free_speech_greet
  - utter_repeat
> check_tennis_comp_Q

<!---------- Question: work harder ---------->
## agree with work harder - Affirmative Action
> check_work_harder_Q
* agree
  - utter_provide_opportunities
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## disagree with work harder - Affirmative Action
> check_work_harder_Q
* disagree
  - utter_most_people_Q
> check_most_people_Q

## Can not understand work harder - Affirmative Action
> check_work_harder_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_work_harder_Q

<!---------- Question: most people ---------->
## agree or disagree with most people - Affirmative Action
> check_most_people_Q
* agree OR disagree
  - utter_provide_opportunities
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand most people - Affirmative Action
> check_most_people_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_most_people_Q

<!-------------------------------------------------------------------------->
<!------------------------------ Free Speech ------------------------------->
<!-------------------------------------------------------------------------->

## start path - Free Speech
* free_speech_greet
  - utter_greet
  - utter_opening
  - utter_openning_Q
> check_openning_Q

<!---------- Question: openning question ---------->
## agree or disagree with openning question - Free Speech
> check_openning_Q
* agree OR disagree
  - utter_free_speech_intro
  - utter_free_speech_believe_Q
> check_free_speech_believe_Q

## Can not understand openning question - Free Speech
> check_openning_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_openning_Q

<!---------- Question: free speech ---------->
## believe with "free speech" - Free Speech
> check_free_speech_believe_Q
* agree 
  - utter_imagine_situation_Q
> check_imagine_situation_Q

## not believe with "free speech" - Free Speech
> check_free_speech_believe_Q
* disagree 
  - utter_20_years_Q
> check_utter_20_years_Q

## Can not understand free speech - Free Speech
> check_free_speech_believe_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_free_speech_believe_Q

<!---------- Question: imagine situation ---------->
## agree with "imagine situation" - Free Speech
> check_imagine_situation_Q
* agree 
  - utter_rumour_protect_Q
> check_rumour_protect_Q

## disagree with "imagine situation" - Free Speech
> check_imagine_situation_Q
* disagree 
  - utter_perfectly_comfortable_Q
> check_perfectly_comfortable_Q

## Can not understand imagine situation - Free Speech
> check_imagine_situation_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_imagine_situation_Q

<!---------- Question: imagine situation ---------->
## agree or disagree with rumour protect - Free Speech
> check_rumour_protect_Q
* agree OR disagree
  - utter_abusive_speech_Q
> check_abusive_speech_Q

## Can not understand rumour protect - Free Speech
> check_rumour_protect_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_rumour_protect_Q

<!---------- Question: imagine situation ---------->
## agree or disagree with perfectly comfortable - Free Speech
> check_perfectly_comfortable_Q
* agree OR disagree
  - utter_abusive_speech_Q
> check_abusive_speech_Q

## Can not understand perfectly comfortable - Free Speech
> check_perfectly_comfortable_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_perfectly_comfortable_Q

<!---------- Question: imagine situation ---------->
## agree or disagree with abusive speech - Free Speech
> check_abusive_speech_Q
* agree OR disagree
  - utter_safe_happy_Q
> check_safe_happy_Q

## Can not understand abusive speech - Free Speech
> check_abusive_speech_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_abusive_speech_Q

<!---------- Question: safe happy ---------->
## agree or disagree with safe happy - Free Speech
> check_safe_happy_Q
* agree OR disagree
  - utter_by_majority_Q
> check_by_majority_Q

## Can not understand safe happy - Free Speech
> check_safe_happy_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_safe_happy_Q

<!---------- Question: by majority ---------->
## agree with "by majority" - Free Speech
> check_by_majority_Q
* agree
  - utter_flat_earth_Q
> check_flat_earth_Q

## disagree with "by majority" - Free Speech
> check_by_majority_Q
* disagree
  - utter_informed_decision_Q
> check_informed_decision_Q

## Can not understand by majority - Free Speech
> check_by_majority_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_by_majority_Q

<!---------- Question: flat earth ---------->
## agree or disagree with flat earth - Free Speech
> check_flat_earth_Q
* agree OR disagree
  - utter_informed_decision_Q
> check_informed_decision_Q

## Can not understand flat earth - Free Speech
> check_flat_earth_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_flat_earth_Q

<!---------- Question: informed decision ---------->
## agree with "informed decision" - Free Speech
> check_informed_decision_Q
* agree
  - utter_restrict_misinfo_Q
> check_restrict_misinfo_Q

## disagree with "informed decision" - Free Speech
> check_informed_decision_Q
* disagree
  - utter_climate_catastrophe_Q
> check_climate_catastrophe_Q

## Can not understand informed decision - Free Speech
> check_informed_decision_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_informed_decision_Q

<!---------- Question: restrict misinfo ---------->
## agree or disagree with restrict misinfo - Free Speech
> check_restrict_misinfo_Q
* agree OR disagree
  - utter_spreads_fast_Q
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand restrict misinfo - Free Speech
> check_restrict_misinfo_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_restrict_misinfo_Q

<!---------- Question: climate catastrophe ---------->
## agree or disagree with climate catastrophe - Free Speech
> check_climate_catastrophe_Q
* agree OR disagree
  - utter_spreads_fast_Q
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand climate catastrophe - Free Speech
> check_climate_catastrophe_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_climate_catastrophe_Q

<!---------- Question: 20 years ---------->
## agree with "20 years" - Free Speech
> check_utter_20_years_Q
* agree
  - utter_no_vote_Q
> check_no_vote_Q

## agree with "20 years" - Free Speech
> check_utter_20_years_Q
* disagree
  - utter_free_discuss_Q
> check_free_discuss_Q

## Can not understand 20 years - Free Speech
> check_utter_20_years_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_utter_20_years_Q

<!---------- Question: no vote ---------->
## agree or disagree with no vote - Free Speech
> check_no_vote_Q
* agree OR disagree
  - utter_free_discuss_Q
> check_free_discuss_Q

## Can not understand no vote - Free Speech
> check_no_vote_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_no_vote_Q

<!---------- Question: free discuss ---------->
## agree with "free discuss" - Free Speech
> check_free_discuss_Q
* agree
  - utter_challenge_freely_Q
> check_challenge_freely_Q

## disagree with "free discuss" - Free Speech
> check_free_discuss_Q
* disagree
  - utter_new_ideas_Q
> check_new_ideas_Q

## Can not understand free discuss - Free Speech
> check_free_discuss_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_free_discuss_Q

<!---------- Question: challenge freely ---------->
## agree or disagree with challenge freely - Free Speech
> check_challenge_freely_Q
* agree OR disagree
  - utter_who_restricts_Q
> check_who_restricts_Q

## Can not understand challenge freely - Free Speech
> check_challenge_freely_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_challenge_freely_Q

<!---------- Question: new ideas ---------->
## agree or disagree with new ideas - Free Speech
> check_new_ideas_Q
* agree OR disagree
  - utter_who_restricts_Q
> check_who_restricts_Q

## Can not understand new ideas - Free Speech
> check_new_ideas_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_new_ideas_Q

<!---------- Question: who restricts ---------->
## agree or disagree with who restricts - Free Speech
> check_who_restricts_Q
* agree OR disagree
  - utter_how_right_Q
> check_how_right_Q

## Can not understand new ideas - Free Speech
> check_who_restricts_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_who_restricts_Q

<!---------- Question: how right ---------->
## agree or disagree with how right - Free Speech
> check_how_right_Q
* agree OR disagree
  - utter_censor_certain_Q
> check_censor_certain_Q

## Can not understand how right - Free Speech
> check_how_right_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_how_right_Q

<!---------- Question: censor certain ---------->
## agree with "censor certain" - Free Speech
> check_censor_certain_Q
* agree
  - utter_horrendous_Q
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## disgree with "censor certain" - Free Speech
> check_censor_certain_Q
* disagree
  - utter_totalitarian_Q
> check_totalitarian_Q

## Can not understand censor certain - Free Speech
> check_censor_certain_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_censor_certain_Q

<!---------- Question: totalitarian ---------->
## agree with "totalitarian" - Free Speech
> check_totalitarian_Q
* agree
  - utter_ideas_silenced_Q
> check_ideas_silenced_Q

## disagree with "totalitarian" - Free Speech
> check_totalitarian_Q
* disagree
  - utter_horrendous_Q
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand censor certain - Free Speech
> check_totalitarian_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_totalitarian_Q

<!---------- Question: ideas silenced ---------->
## agree with disagree with ideas silenced - Free Speech
> check_ideas_silenced_Q
* agree OR disagree
  - utter_horrendous_Q
* agree OR disagree OR greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_closing
  - utter_goodbye
  - utter_post_survey
  - utter_post_survey_redirect

## Can not understand ideas silenced - Free Speech
> check_ideas_silenced_Q
* greet OR goodbye OR bot_challenge OR aff_action_greet OR choose_one OR not_choose_one OR answer_tennis_comp OR free_speech_greet
  - utter_repeat
> check_ideas_silenced_Q

<!---------- Gun Laws ---------->

<!---------- Abortion / Pro-Life Movement ---------->

<!---------- Vaccination ---------->