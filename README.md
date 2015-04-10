alias "Tiny" "cl_crosshairalpha 255;cl_crosshaircolor 5;cl_crosshaircolor_b 255;cl_crosshaircolor_r 255;cl_crosshaircolor_g 0;cl_crosshairdot 0;cl_crosshairgap -6;cl_crosshairsize 4;cl_crosshairstyle 3;cl_crosshairusealpha 1;cl_crosshairthickness 0.5;cl_fixedcrosshairgap -6;cl_crosshair_outlinethickness 0;cl_crosshair_drawoutline 0;" //&bind_1
alias "binds" "echo 'KP_SLASH': Crosshair 'Tiny';"
alias "White" "cl_crosshairalpha 255;cl_crosshaircolor 5;cl_crosshaircolor_b 255;cl_crosshaircolor_r 255;cl_crosshaircolor_g 253;cl_crosshairdot 0;cl_crosshairgap -3;cl_crosshairsize 4;cl_crosshairstyle 3;cl_crosshairusealpha 1;cl_crosshairthickness 0.5;cl_fixedcrosshairgap -1;cl_crosshair_outlinethickness 0;cl_crosshair_drawoutline 0;" //&bind_2
alias "Pink" "cl_crosshairalpha 255;cl_crosshaircolor 5;cl_crosshaircolor_b 255;cl_crosshaircolor_r 255;cl_crosshaircolor_g 0;cl_crosshairdot 0;cl_crosshairgap -2;cl_crosshairsize 3;cl_crosshairstyle 3;cl_crosshairusealpha 1;cl_crosshairthickness 0.5;cl_fixedcrosshairgap -2;cl_crosshair_outlinethickness 0;cl_crosshair_drawoutline 0;" //&bind_3
alias "Big_Pink" "cl_crosshairalpha 255;cl_crosshaircolor 5;cl_crosshaircolor_b 255;cl_crosshaircolor_r 255;cl_crosshaircolor_g 0;cl_crosshairdot 0;cl_crosshairgap 2;cl_crosshairsize 6;cl_crosshairstyle 3;cl_crosshairusealpha 1;cl_crosshairthickness 0.5;cl_fixedcrosshairgap 2;cl_crosshair_outlinethickness 0;cl_crosshair_drawoutline 0;" //&bind_4
alias "dynamic_white" "cl_crosshairalpha 255;cl_crosshaircolor 5;cl_crosshaircolor_b 255;cl_crosshaircolor_r 255;cl_crosshaircolor_g 0;cl_crosshairdot 0;cl_crosshairgap -6;cl_crosshairsize 4;cl_crosshairstyle 4;cl_crosshairusealpha 1;cl_crosshairthickness 0.5;cl_fixedcrosshairgap -6;cl_crosshair_outlinethickness 0;cl_crosshair_drawoutline 0;" //&bind_5



alias "binds" "echo 'KP_PGUP': Crosshair 'dynamic_white';"

bind "KP_SLASH" "Tiny" // Chrosshair 'Tiny'
bind "KP_MULTIPLY" "White" // Chrosshair 'White'
bind "KP_MINUS" "Pink" // Chrosshair 'Pink'
bind "KP_PLUS" "Big_Pink" // Chrosshair 'Big_Pink'
bind "KP_PGUP" "dynamic_white" // Chrosshair 'dynamic_white'
bind MWHEELUP "cl_righthand 0" ;bind MWHEELDOWN "cl_righthand 1"

alias "binds" "echo 'KP_SLASH': Crosshair 'Green';echo 'KP_MULTIPLY': Crosshair 'White';echo 'KP_MINUS': Crosshair 'Pink';echo 'KP_PLUS': Crosshair 'Big_Pink'; echo 'KP_PGUP': Crosshair 'dynamic_white';"

bind f1 "buy m4a1; buy m4a4; buy ak47;"
bind f2 "buy smokegrenade;buy flashbang; buy hegrenade; buy flashbang;"
bind f3 "buy p250;"
bind "k" "buy vesthelm;"
bind "l" "buy vest;"
bind "j" "buy defuser;"

fps_max "250"
windows_speaker_config "1"

//Auto Weapon Switch
cl_autowepswitch "0" // we dont want to pick up & switch to a rifle up if we're in the middle of firing our pistol

//Bobbing and Movement Shifting - remove all the dumb view bob
cl_viewmodel_shift_left_amt "0"
cl_viewmodel_shift_right_amt "0"
cl_bob_lower_amt "0"
cl_bobamt_lat "0"
cl_bobamt_vert "0"
cl_showloadout "1"
cl_bobcycle "1"

//Bypass OS Interface & Acceleration - yes
m_rawinput "1"
m_mouseaccel1 "0"
m_mouseaccel2 "0"

//Deathcam - optional again
cl_disablefreezecam "1"
cl_freezecameffects_showholiday "1"

//Gun Tracers - these are bad, really misleading
r_drawtracers_firstperson "0"

//Help Messages - you dont need these
gameinstructor_enable "0"
cl_autohelp "0"
cl_showhelp "0"

//HUD - adjust for preference i guess
hud_scaling ".95"
hud_showtargetid "1"
net_graph 1
net_graphproportionalfont 0

//Max Ping - adjust for preference
mm_dedicated_search_maxping "100" // we dont wanna get put in a server where we have 200 ping

//MOTD - because ???? pinion
cl_disablehtmlmotd "1"
cl_downloadfilter "nosounds"

//Performance & Rates - rates for 128 tick servers, matchmaking is 64 but this is usually fine
cl_forcepreload "1"
cl_interp "0"
cl_interp_ratio "1"
cl_cmdrate "128"
cl_updaterate "128"
rate "128000"

//Radar - radar settings + adjustment on numpad enter
cl_radar_rotate "0"
cl_radar_always_centered "0"
cl_radar_scale "0.32"
cl_radar_icon_scale_min "0.5"
bind "kp_enter" "incrementvar cl_radar_scale 0.32 0.52 0.05" // this lets you adjust radar scale on numpad enter


echo "LOADED"
echo "Autoexec Config loaded" // make sure this autoexec does its fines
host_writeconfig
