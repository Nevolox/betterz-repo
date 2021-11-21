
:root {
						
    --BannerBG-Header-Height: block;
    --BannerBG-Header-Padding: 16px;
    --BannerBG-Header-Box-Shadow: revert;	

    --BannerBG-Server-Banner: block;
    --BannerBG-Server-Width: block;
    --BannerBG-Server-Height: block;
    --BannerBG-Server-Top: block;
    --BannerBG-Server-Left: block;
    --BannerBG-Server-Z-Index: block;
    --BannerBG-Server-Position: block;
    --BZTcolor:     rgba(194,35,247,1);
    --BZTcolor2:     rgba(106,25,140,1);


}



.username-1A8OIy, .headerName-fajvi9, .usernameFont-23TX-h, .headerNameWrapper-3res2c{
	font-weight: 1000 !important;
	transition: filter .1s ease-in-out .1s;
	filter: brightness(0.95) invert(0) !important;
	text-shadow: 0px 0px 5px;
	}
	
	.username-1A8OIy:hover, .headerName-fajvi9:hover, .usernameFont-23TX-h:hover, .headerNameWrapper-3res2c:hover {
	filter: brightness(1500) invert(0) !important;
	}


/*Glowing unread servers*/
@keyframes unreadRainbow { /*animation*/
	50% {
		background-position: 100% 50%;
	}
	}
	.wrapper-25eVIn foreignObject { /*Round server channels*/
	mask: unset;
	border-radius: 1000%;
	}
	.pill-1z4sAY { /*Makes ring visible*/
	overflow: visible!important;
	}
	.item-2hkk8m[style*="height: 8px"]::before { /*Unread server ring*/
	content: '';
	position: absolute;
	top: -22px;
	left: 14px;
	width: 52px;
	height: 52px!important;
	border-radius: 41%;
	background: linear-gradient(120deg,
	rgb(0,64,255),
	rgb(0,64,255),
	rgb(0,64,255),
	rgb(128, 0, 255),
	rgb(255, 0, 0),
	rgb(255, 145, 0),
	rgb(2, 190, 2),
	rgb(0,64,255),
	rgb(128, 0, 255),
	rgb(255, 0, 0),
	rgb(255, 145, 0),
	rgb(2, 190, 2),
	rgb(0, 0, 0)
	);
	background-size: 200% 200%;
	background-position: 0 50%;
	animation: unreadRainbow 4s infinite;
	transition: 0.25s ease;
	}
	.wrapper-1BJsBx { /*Matches png server icons with default background*/
	background-color: var(--background-tertiary);
	}

	.reaction-1hd86g{
		background: -webkit-linear-gradient(120deg, rgba(138, 157, 224, 0.125), rgba(255, 255, 255, 0.152));

		border-color: #67686a;
		border-width: 2px;
		border-radius: 2px;
		}
		.reaction-1hd86g:hover{
		background: -webkit-linear-gradient(80deg, rgb(146, 191, 221), rgb(255, 255, 255));

		}
		.reaction-1hd86g:hover{
		background: -webkit-linear-gradient(120deg, rgba(138, 157, 224, 0.125), rgba(255, 255, 255, 0.152));

		}


			.avatar-1BDn8e.clickable-1bVtEA { 
				filter: drop-shadow(0 0 3px);
				color: pink;
				}
				
				.avatar-1BDn8e:hover.clickable-1bVtEA:hover {
				filter: drop-shadow(0 0 8px);
				color: pink;
				transform: rotate(360deg);
				transition: width .5s ease, height .5s ease, transform .5s ease;
				}


				.clickableSticker-3HmpgV > div .assetWrapper-3GNt0z {
					width: 100px !important;
					height: 100px !important;
					}


					#app-mount .titleBar-AC4pGV {
						z-index: 5;
						background-color: var(--background-secondary);
						border-radius: var(--border-radius);
						margin-top: var(--separation-padding);
						margin-right: var(--separation-padding);
						margin-left: var(--separation-padding);
						padding-top: 2px;
					}
					#app-mount .titleBar-AC4pGV .wordmark-2iDDfm::after {
						content: "Better-Cord";
						position: absolute;
						font-family: "IMPACT";
						background: -webkit-gradient(linear, right top, left top, color-stop(60%, var(--BZTcolor)), to(#FEAC5E));
						background: linear-gradient(270deg, var(--BZTcolor) 70%, var(--BZTcolor2));
						-webkit-background-clip: text;
						-webkit-text-fill-color: transparent;
						background-clip: text;
						background-size: 200% 200%;
						font-size: 16px;
						font-weight: 600;
						top: 5px;
						left: 30px;
						width: 135px;
					}
					#app-mount .titleBar-AC4pGV{
						background: var(--icon) 4px 0/13px 15px no-repeat;
						background-size: 1.08% 100%;

					}

					#app-mount .wordmark-2iDDfm svg  {
						width: 0;
					}
					
					#app-mount .titleBar-AC4pGV .winButton-iRh8-Z {
						background: 8px 0/13px 15px no-repeat;
						opacity: 0.75;
						margin-top: 4px;
						-webkit-transition: all 0.2s ease;
						transition: all 0.2s ease;
					}



					
					/* BannerBG Main Code */
					[class*="container-3w7J-x"] [class*="header-2V-4Sw"] {
						height: var(--BannerBG-Header-Height);
						padding: var(--BannerBG-Header-Padding);
						box-shadow: var(--BannerBG-Header-Box-Shadow);
						align-items: flex-start;
					}
					
					[class*="container-3w7J-x"] [class*="header-2V-4Sw"]::before {
						content: "";
						position: var(--BannerBG-Server-Position);
						top: var(--BannerBG-Server-Top);
						left: var(--BannerBG-Server-Left);
						z-index: var(--BannerBG-Server-Z-Index);
						width: var(--BannerBG-Server-Width);
						height: var(--BannerBG-Server-Height);
						background: var(--BannerBG-Server-Banner) center/cover no-repeat;

					}
					
					/* Shrink server banners to header instead of disappearing. */
					[class*="animatedContainer-"] {
						opacity: 1 !important;
						transition: opacity .5s;
					}
					
					[class*="animatedContainer-"] > [class*="bannerImage-"] {
						transition: margin .5s;
					}
					
					:not([class*="bannerVisible-"]) > [class*="animatedContainer-"] {
						opacity: .35 !important;
						height: 138px;
					}
					
					:not([class*="bannerVisible-"]) > [class*="animatedContainer-"] > [class*="bannerImage-"] {
						margin-top: -12px;
					}


/* Custom Server Banner*/
[aria-label*="beebees"] {

	--BannerBG-Header-Height: 150px !important;
	--BannerBG-Header-Padding: 16px !important;
	--BannerBG-Header-Box-Shadow: none !important;

	--BannerBG-Server-Banner: url("https://media1.giphy.com/media/3SBS7bYonp2QU/giphy.gif") !important;
	--BannerBG-Server-Width: 100% !important;
	--BannerBG-Server-Height: 100% !important;
	--BannerBG-Server-Top: 0 !important;
	--BannerBG-Server-Left: 0 !important;
	--BannerBG-Server-Z-Index: -1 !important;
	--BannerBG-Server-Position: absolute !important;

}

[aria-label*="JIFF-SQUAD"] {

	--BannerBG-Header-Height: 150px !important;
	--BannerBG-Header-Padding: 16px !important;
	--BannerBG-Header-Box-Shadow: none !important;

	--BannerBG-Server-Banner: url("https://media1.giphy.com/media/3SBS7bYonp2QU/giphy.gif") !important;
	--BannerBG-Server-Width: 100% !important;
	--BannerBG-Server-Height: 100% !important;
	--BannerBG-Server-Top: 0 !important;
	--BannerBG-Server-Left: 0 !important;
	--BannerBG-Server-Z-Index: -1 !important;
	--BannerBG-Server-Position: absolute !important;

}



/* base color variables */
.theme-dark {
    --accent-color: hsl(283, 60%, 50%);
    --accent-color-2: hsl(283, 60%, 50%);
    --accent-color-3: hsl(283, 60%, 50%);
    --link-color: hsl(190, 90%, 50%);
    --mention-background: rgba(143, 51, 204, 0.3);
    --mentioned-background: hsla(290, 60%, 50%, 0.1);
    --mentioned-hover-background: hsla(190, 60%, 50%, 0.08);
    --primary-text: hsl(220, 15%, 60%);
    --secondary-text: hsl(220, 15%, 40%);
    --muted-text: hsl(220, 15%, 20%);
    --primary-background: hsl(223, 14%, 10%);
    --secondary-background: hsl(220, 15%, 13%);
    --accent-background: hsl(220, 15%, 16%);
    --scrollbar-color: hsl(220, 15%, 11%);
    --hover-modifier: hsla(220, 15%, 20%, .1);
    --active-modifier: hsla(220, 15%, 20%, .2);
    --selected-modifier: hsla(220, 15%, 20%, .3);
	--icon: url("https://cdn.discordapp.com/attachments/647508440721260544/830566346286563328/floatingisland.gif")!important;
}

/* change colors */
.theme-dark {
    --brand-experiment: var(--accent-color);

    --header-primary: var(--primary-text);
    --header-secondary: var(--secondary-text);
    --text-normal: var(--primary-text);
    --text-muted: var(--muted-text);
    --text-link: var(--link-color);
    --text-link-low-saturation: var(--link-color);
    --interactive-normal: var(--secondary-text);
    --interactive-hover: var(--primary-text);
    --interactive-active: var(--primary-text);
    --interactive-muted: var(--muted-text);
    --background-primary: var(--primary-background);
    --background-secondary: var(--secondary-background);
    --background-secondary-alt: var(--secondary-background);
    --background-tertiary: var(--secondary-background);
    --background-accent: var(--accent-background);
    --background-floating: var(--primary-background);
    --background-mobile-primary: var(--primary-background);
    --background-mobile-secondary: var(--secondary-background);
    --background-modifier-hover: var(--hover-modifier);
    --background-modifier-active: var(--active-modifier);
    --background-modifier-selected: var(--selected-modifier);
    --background-modifier-accent: var(--selected-modifier);
    --scrollbar-thin-thumb: var(--scrollbar-color);
    --scrollbar-thin-track: transparent;
    --scrollbar-auto-thumb: var(--scrollbar-color);
    --scrollbar-auto-track: transparent;
    --scrollbar-auto-scrollbar-color-thumb: var(--scrollbar-color);
    --scrollbar-auto-scrollbar-color-track: transparent;
    --elevation-stroke: 0 0 4px 1px hsla(0, 0%, 0%, 0.15);
    --elevation-low: none;
    --elevation-medium: 0 4px 8px hsla(0, 0%, 0%, 0.2);
    --elevation-high: 0 4px 8px hsla(0, 0%, 0%, 0.3);
    --guild-header-text-shadow: 0 1px 1px rgba(0, 0, 0, 0.4);
    --background-mentioned: var(--mentioned-background);
    --background-mentioned-hover: var(--mentioned-hover-background);
    --background-message-hover: var(--hover-modifier);
    --channels-default: var(--secondary-text);
    --channeltextarea-background: var(--secondary-background);
    --activity-card-background: var(--secondary-background);
    --textbox-markdown-syntax: var(--secondary-text);
    --info-warning-foreground: var(--accent-color);
    --brand-experiment-30a: var(--mention-background);
    --brand-experiment-600: var(--accent-color-3);
    --brand-experiment-560: var(--accent-color-2);
    --brand-experiment-360: var(--accent-color);
}

/* force elements to use colors variables */
.peopleColumn-29fq28,
.uploadModal-2ifh8j,
.pageWrapper-1PgVDX,
.message-2qRu38,
.root-1gCeng,
.container-3ayLPN,
.autocomplete-1vrmpx,
.categoryHeader-O1zU94 {
    background-color: var(--background-primary) !important;
}

.selected-1Tbx07,
.selected-rZcOL- {
    background-color: var(--background-modifier-selected) !important;
}
