#Shadows
shadow = false; # Enabled client-side shadows on windows
no-dnd-shadow = true; # Avoid drawing shadows on dock/panel windows.
no-dock-shadow = true; # Don't draw shadows on DND windows.
clear-shadow = true; # Zero the part of the shadow's mask behind the window (experimental).
shadow-radius = 7; # The blur radius for shadows. (default 12)
shadow-offset-x = -7; # The left offset for shadows. (default -15)
shadow-offset-y = -7; # The top offset for shadows. (default -15)
shadow-opacity = 0.7; # The translucency for shadows. (default .75)
shadow-red = 0.0; # Red color value of shadow. (0.0 - 1.0, defaults to 0)
shadow-green = 0.0; # Green color value of shadow. (0.0 - 1.0, defaults to 0)
shadow-blue = 0.0; # Blue color value of shadow. (0.0 - 1.0, defaults to 0)
shadow-exclude = [ "name = 'Notification'", "class_g = 'Conky'", "class_g ?= 'Notify-osd'", "class_g = 'Cairo-clock'" ]; # Exclude conditions for shadows.
shadow-ignore-shaped = false;
xinerama-shadow-crop = false;

#Opacity
menu-opacity = 1; # The opacity for menus. (default 1.0)
inactive-opacity = 1; # Opacity of inactive windows. (0.1 - 1.0)
active-opacity = 1; # Opacity of window titlebars and borders. (0.1 - 1.0)
frame-opacity = 1; # Opacity of frames. (0.1 - 1.0)
inactive-opacity-override = false; # Inactive opacity set by 'inactive-opacity' overrides value of _NET_WM_OPACITY.
alpha-step = 0.06;

#Fade
fading = false; # Fade windows during opacity changes.
fade-in-step = 0.03; # Opacity change between steps while fading in. (default 0.028).
fade-out-step = 0.03; # Opacity change between steps while fading out. (default 0.03).
fade-exclude = [ ];

#Other
inactive-dim = 0.0;
blur-kern = "3x3box";
blur-background-exclude = [ "window_type = 'dock'", "window_type = 'desktop'" ];
backend = "xrender";
mark-wmwin-focused = true;
mark-ovredir-focused = true;
detect-rounded-corners = true;
detect-client-opacity = true;
refresh-rate = 0;
vsync = "none";
dbe = false;
paint-on-overlay = true;
focus-exclude = [ "class_g = 'Cairo-clock'" ];
detect-transient = true;
detect-client-leader = true;
invert-color-include = [ ];
glx-copy-from-front = false;
glx-swap-method = "undefined";
wintypes : 
{
  tooltip : 
  {
    fade = true;
    shadow = false;
    opacity = 0.75;
    focus = true;
  };
};
