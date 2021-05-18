/**
* @name         Poison
* @description  Enjoy Discord with a stylish dark theme with vibrant green elements.
* @donate       https://bit.ly/3fnzq1Z
* @source       https://github.com/rmkx/rmkx.github.io/blob/main/Poison/src/poison.css
* @author       rmkx
* @invite       HnGWVQbQBv
* @version      1.0.1 
*/

@import url('https://rmkx.github.io/src/settingsIcons.css');
@import url('https://rmkx.github.io/src/customBadges.css');

:root {
    /*Background settings*/
    --background-image: url('https://i.imgur.com/B5pCrRt.jpg'); /*Background image*/
    --menu-bg: url('https://i.imgur.com/pvk9Zir.png'); /*Background image for some panels, like right click*/
    --bg-blur: 0px; /*Background blur | Default 0px*/
    --bg-opacity: 0.4; /*Background opacity | Default 0.4*/

    /*Server member panel*/
    --members-hiding: 80%; /*Position of the members panel when it hides | Default 80%*/
    --members-showing: 0%; /*Position of the members panel when it shows | Default 0%*/
    --transition-speed: 0.35s; /*Changes the showing speed | Default 0.35s*/

    /*General settings*/
    --general-radius: 5px; /*Changes the radius of most modals | Default 5px*/
    --main-color: 52, 52, 52; /*Main color of the theme | WARNING: USE RGB VALUES IF YOU CHANGE THE COLOR | Default 52, 52, 52*/
    --main-accent: 147, 227, 32; /*Theme accent color | WARNING: USE RGB VALUES IF YOU CHANGE THE COLOR | Default 147, 227, 32*/
    --avatar-radius: 5px; /*Avatar's radius | Default 5px*/
    --links-color:  147, 227, 32; /*Changes the color of the links | Default 147, 227, 32*/
    --settings-width: 60%; /*Width for the settings window | Default 60%*/
    --settings-heigth: 85%; /*Width for the settings window | Default 85%*/
    --embed-border: 0px; /*Border for some of the embeds | Default 0px*/
    --embed-bg: rgba(0,0,0,0.75); /*Embeds background | Default rgba(0, 0, 0, 0.75)*/
    --selection-bg: rgba(52, 52, 52, 0.6); /*Changes the background of the selected text | Default rgba(52, 52, 52, 0.6)*/
    --selection-color: rgba(var(--main-accent), 1); /*Changes the color of the selected text | Default rgba(var(--main-accent), 1)*/
    --scrollbar-color: rgba(var(--main-accent), 0.4); /*Changes the color of the scrollbar | Default rgba(var(--main-accent), 0.4)*/
    --icon-padding: 35px; /*Changes the padding between the icon and the text | Default 35px*/


    /*Font*/
    --font: 'Fjalla One', sans-serif; /*Main font*/
    --message-size: 90%; /*Chat message font size | Default 90%*/
}

.theme-dark,
.theme-light {
    --channels-default: white;
    --text-muted: rgb(255, 255, 255);
    --background-floating: black;
    --header-secondary: rgb(160, 162, 165);
    --text-link: rgb(var(--links-color));
}

/*Theme font*/
::-webkit-input-placeholder, body, button, input, select, textarea {
    font-family: var(--font);
}

/*Selected text settings*/

::selection { 
    background-color: var(--selection-bg)!important;
    color: var(--selection-color)!important;
}

/*Scrollbar settings*/

::-webkit-scrollbar-thumb { /*Scrollbar thumb*/
    background-color: var(--scrollbar-color)!important;
    border-radius: 20px!important;
}
::-webkit-scrollbar-track,
.scroller-zPkAnE::-webkit-scrollbar-track { /*Scrollbar track*/
    background-color: transparent!important;
    border-radius: var(--general-radius)!important;
}

/*Background*/

.chat-3bRxxu {
    background: rgba(0,0,0,1);
}
.chat-3bRxxu::before {
    content: "";
    background: var(--background-image);
    background-position: center;
    background-size: cover;
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    filter: blur(var(--bg-blur));
    opacity: var(--bg-opacity);
}
.container-1D34oG::before {
    content: "";
    background: var(--background-image);
    background-position: center;
    background-size: cover;
    position: absolute;
    top: 0;
    left: inherit;
    height: 100%;
    width: 87.5%;
    filter: blur(var(--bg-blur));
    opacity: var(--bg-opacity);
}

/*Server members settings*/

.membersWrap-2h-GB4::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgb(var(--main-color));
    filter: brightness(0.3);
}
.members-1998pB { /*Main container*/
    background: transparent;
}
.members-1998pB .content-3YMskv { /*Member container*/
    background: transparent;
    position: absolute;
    width: 100%;
}
.membersGroup-v9BXpm:first-of-type { /*First role*/
    margin-top: 2%;
}
.membersGroup-v9BXpm { /*Member role*/
    margin-top: 4%;
    margin-bottom: 1%;
    text-align: center;
    height: 25px;
    padding: 0px;
}
.membersWrap-2h-GB4 { /*Server member panel*/
    z-index: 2;
}
.membersWrap-2h-GB4:hover .membersGroup-v9BXpm,
.membersGroup-v9BXpm { /*Member role when hovering panel*/
    color: rgb(var(--main-accent));
    filter: brightness(0.85)
}
.membersWrap-2h-GB4 .membersGroup-v9BXpm::after { /*Line after member role*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 8px;
    left: 35px;
    width: 150px;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.membersWrap-2h-GB4 .membersGroup-v9BXpm::before { /*Line after member role 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 13px;
    left: 50px;
    width: 150px;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.botTagRegular-2HEhHi { /*Bot tag*/
    background-color: rgba(var(--main-accent), 0.35);
    color: white;
}

@keyframes memberSelected {
    0% {
        filter: brightness(0.25);
    }
    100% {
        filter: brightness(1);
    } 
}
.membersWrap-2h-GB4 .clickable-1JJAn8.container-2Pjhx- { /*Main member container*/
    background: transparent;
    transform: translateX(0px);
    transition:  0.25s ease-in;
}
.membersWrap-2h-GB4 .clickable-1JJAn8.container-2Pjhx-::after { /*Main member container underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 74%;
    background: transparent;
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transform: translateX(0%);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.membersWrap-2h-GB4 .clickable-1JJAn8.container-2Pjhx-:hover { /*Main member container hovered*/
    background-color: transparent;
    transform: translateX(12px);
    transition:  0.25s ease-in;;
}
.membersWrap-2h-GB4 .clickable-1JJAn8.container-2Pjhx-:hover::after { /*Main member container hovered underline*/
    content: '';
    position: absolute;
    left: 0%;
    bottom: 0;
    height: 1px;
    width: 74%;
    background: rgb(var(--main-accent));
    border-color: transparent;
    transform: translateX(30%);
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.membersWrap-2h-GB4 .selected-aXhQR6.container-2Pjhx- { /*Selected server member*/
    background-color: transparent;
    transform: translateX(12px);
}
.membersWrap-2h-GB4 .selected-aXhQR6.container-2Pjhx-::after { /*Selected server member underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 83%;
    transform: translateX(26.5%);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent)); 
    animation: memberSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.membersWrap-2h-GB4 .clickable-1JJAn8:hover .layout-2DM8Md ,
.membersWrap-2h-GB4 .selected-aXhQR6 .layout-2DM8Md { /*Member subcontainer*/
    background-color: transparent   ;
}

/*Chat settings*/

@keyframes glowArea { 
    0% {
        box-shadow: 0px 0px 0px 0px inset transparent;
    }
    100% {
        box-shadow: 0px 0px 3px 3px inset rgb(var(--main-accent));
        filter: brightness(0.65);
    }
}
@keyframes glowAreaUnfocus {
    0% {
        box-shadow: 0px 0px 3px 3px inset rgb(var(--main-accent));
        filter: brightness(0.65);
    }
    100% {
        box-shadow: 0px 0px 0px 0px inset transparent;
    }
}
.wrapper-39oAo3 { /*Follow for updates chatbox*/
    background-color: transparent;
}
.channelTextArea-rNsIhG,
.scrollableContainer-2NUZem { /*Chat containers*/
    background-color: transparent;
    border-radius: var(--general-radius);
}
.scrollableContainer-2NUZem::before { /*Chat container background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.25);
}
.scrollableContainer-2NUZem::after { /*Chat container glow*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: var(--general-radius);
    animation: glowAreaUnfocus 0.25s ease;
    animation-fill-mode: forwards;
    z-index: 0;
}
.scrollableContainer-2NUZem:focus-within::after { /*Chat container glow*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: var(--general-radius);
    animation: glowArea 0.25s ease;
    animation-fill-mode: forwards;
    z-index: 0;
}
.uploadInput-1XtQef,
.sansAttachButton-td2irx,
.attachButton-2dnuIu,
.textArea-12jD-V,
.buttons-3JBrkn { /*Chat containers*/
    z-index: 1;
}
.wrapper-3vR61M,
.wrapper-1F5TKx { /*Chat loading messages*/
    background:transparent
}
.form-2fGMdU {
    background-color: transparent;
}
.form-2fGMdU::before {
    background: transparent!important;
}
.container-1r6BKw.themed-ANHk51,
.children-19S4PO::after,
.divider-3FBTu8 { /*Channel chat title*/
    background: transparent!important;
}
.content-yTz4x3::before { /*Annoying line before chat*/
    box-shadow: unset;
}
.emojiButton-3uL3Aw { /*Emoji button*/
    margin-right: 20px;
}
.repliedMessage-VokQwo:before { /*Replied message bar from avatar to avatar*/
    border-left: var(--spine-width) solid rgba(var(--main-accent), 0.4);
    border-bottom: 0 solid rgba(var(--main-accent), 0.4);
    border-right: 0 solid rgba(var(--main-accent), 0.4);
    border-top: var(--spine-width) solid rgba(var(--main-accent), 0.4);
}
.divider-JfaTT5.isUnread-3Ef-o9 { /*New messages line*/
    background: transparent;
    border-top: none;
}
.divider-JfaTT5.isUnread-3Ef-o9::before { /*New messages line effect 1*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: -5px;
    left: 300px;
    width: 62.5%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.divider-JfaTT5.isUnread-3Ef-o9::after { /*New messages line effect 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: -10px;
    left: 315px;
    width: 62.5%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.unreadPill-2HyYtt { /*New message unread tag*/
    background-color: rgba(var(--main-accent), 0.45);
}
.unreadPillCapStroke-7rkHbg { /*New message unread tag 2*/
    color: rgba(var(--main-accent), 0.45);
    fill: rgba(var(--main-accent), 0.45);
}
.divider-JfaTT5 { /*New day divider*/
    border-top: unset;
}
.group-spacing-16 .divider-3_HH5L.hasContent-1_DUdQ .content-1o0f9g { /*Day text with no new messages*/
    color: white;
    background: transparent;
}
.group-spacing-16 .divider-3_HH5L.hasContent-1_DUdQ .content-1o0f9g::before { /*Line before the day with no new messages*/
    content: '';
    position: absolute;
    left: 0%;
    top: -1px;
    width: 46%;
    height: 1px;
    background: rgb(var(--main-accent));
    filter: brightness(0.65);
}
.group-spacing-16 .divider-3_HH5L.hasContent-1_DUdQ .content-1o0f9g::after{ /*Line after the day with no new messages*/
    content: '';
    position: absolute;
    right: 0%;
    top: -1px;
    width: 46%;
    height: 1px;
    background: rgb(var(--main-accent));
    filter: brightness(0.65);
}
.group-spacing-16 .divider-3_HH5L.hasContent-1_DUdQ.isUnread-3Ef-o9 .content-1o0f9g { /*New message on new day*/
    color: white;
    background: transparent;
}
.group-spacing-16 .divider-3_HH5L.hasContent-1_DUdQ.isUnread-3Ef-o9::before { /*New message on new day line 1*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 5px;
    left: 300px;
    width: 62.5%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.group-spacing-16 .divider-3_HH5L.hasContent-1_DUdQ.isUnread-3Ef-o9::after { /*New message on new day line 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 0px;
    left: 315px;
    width: 62.5%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85); 
}
.group-spacing-16 .divider-3_HH5L.hasContent-1_DUdQ.isUnread-3Ef-o9 .unreadPill-2HyYtt { /*New message on new day tag*/
    top: 5px;
}
.colorBrand-2tjs5J { /*Ping button ON*/
    color: rgba(var(--main-accent), 0.85);
}
.colorMuted-HdFt4q { /*Ping button OFF*/
    color: rgba(var(--main-color), 1);
    filter: brightness(3);
}
.separator-ju-9xl { /*Reply separator*/
    display: none;
}
.replying-1x3H0T,
.mentioned-xhSam7 { /*Replying to message*/
    background-color: transparent;
}
.replying-1x3H0T::before,
.mentioned-xhSam7::before { /*Replying to message line before*/
    position: absolute;
    top: 100%;
    left: 3.5%;
    width: 95%;
    height: 1px;
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 5px 1px rgb(var(--main-accent));
    filter: brightness(0.85);
}
.replying-1x3H0T::after,
.mentioned-xhSam7::after { /*Replying to message background*/
    content: '';
    position: absolute;
    top: 5.5%;
    left: 70.2%;
    transform: translateX(-71%) translateY(-5.5%);
    height: 100%;
    width: 97.5%;
    border-radius: var(--general-radius);
    background: rgba(var(--main-accent), 0.05);
    filter: brightness(1);
    z-index: -1;
}
.mentioned-xhSam7:hover,
.mentioned-xhSam7.selected-2P5D_Z { /*Hovered mention*/
    background-color: rgba(0,0,0,0.45)!important;
}
.mouse-mode.full-motion .message-2qnXI6:hover { /*Hovered message in chat*/
    background-color: rgba(0,0,0,0.45);
}
.embedFull-2tM8-- { /*Chat embed*/
    border-radius: var(--general-radius);
    border-left: var(--embed-border) solid;
    background-color: var(--embed-bg);
}
.markup-2BOw-j .wrapper-3WhCwL { /*Chat mention*/
    background-color: transparent;
    color: rgb(var(--main-accent));
}
.topic-TCb_qw.expandable-9fI_e3 .wrapper-3WhCwL{ /*Chat title mention*/
    background-color: transparent;
    color: rgb(var(--main-accent));
    filter: brightness(1.2);
}
.autocomplete-1vrmpx { /*Autocomplete modal*/
    background: transparent!important;
}
.autocompleteInner-zh20B_::after { /*Autocomplete modal*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.3);
    width: 100%;
    z-index: -1;
}
.newMessagesBar-265mhP,
.jumpToPresentBar-G1R9s6 { /*New message & jump to present bars*/
    background-color: transparent;
    border-top-left-radius: 0px;
    border-top-right-radius: 0px;
    opacity: 1;
}
.newMessagesBar-265mhP::before { /*New message bar*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    border-top-left-radius: 0px;
    border-top-right-radius: 0px;
    filter: brightness(0.3);
    width: 100%;
    z-index: -1;
}
.newMessagesBar-265mhP::after { /*New message bar*/
    content: '';
    position: absolute;
    bottom: 5%;
    left: 0.5%;
    color: white;
    height: 0.5px;
    width: 99%;
    background: rgb(var(--main-accent));
    border-radius: var(--general-radius);
    box-shadow: 0px 0px 0.5px 0.5px rgb(var(--main-accent));
    filter: brightness(0.55);
}
.jumpToPresentBar-G1R9s6::before { /*Jump to present messages bar*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.3);
    width: 100%;
    z-index: -1;
}
.blockquoteDivider-2hH8H6 { /*Chat quote*/
    background-color: rgb(var(--main-accent));
    filter: brightness(0.65)
}
.wrapper-2aW0bm,
.full-motion .wrapper-2aW0bm:hover { /*Reply to message/More options button wrapper*/
    box-shadow: unset;
    background-color: transparent;
}
.wrapper-2aW0bm .button-1ZiXG9:hover { /*Reply to message/More options buttons*/
    background-color: transparent;
    color: rgb(var(--main-accent), 0.85);
    transition: color 0.25s ease
}
.wrapper-2aW0bm .button-1ZiXG9.selected-LCBEAU { /*Reply to message/More selected button*/
    background-color: transparent;
    color: rgb(var(--main-accent), 1);
    transition: color 0.25s ease
}
.wrapper-uf3cnO,
.wrapper-2Gsate,
.categoryHeader-O1zU94 { /*Command panel containers*/
    background-color: transparent;
}
.wrapper-2siovq:hover { /*Hovered category*/
    background-color: transparent;

}
.wrapper-2siovq .icon-2VCx8O { /*Category icon*/
    filter: brightness(0.3);
    transition: 0.25s ease;
}
.wrapper-2siovq:hover .icon-2VCx8O { /*Hovered category icon*/
    color: rgba(var(--main-accent), 0.35);
    transition: color 0.25s ease;
}
.wrapper-2siovq.selected-3xBBKs { /*Selected category*/
    background-color: transparent!important;
}
.selected-3xBBKs .icon-2VCx8O { /*Selected category icon*/
    color: rgba(var(--main-accent), 1)!important;
    filter: brightness(1);
    transition: 0.25s ease;
}
.selectable-3dP3y-.selected-1Tbx07{ /*Command panel hovered*/
    background-color: rgba(var(--main-color), .25)!important;
}
.optionalHeader-mLQoIx { /*Divider after hovered option*/
    border-color: transparent;
}
.option-1B5ZV8 { /*Command pannel hint*/
    background-color: transparent!important;
}
.builtInSeparator-1ku6s5 { /*Left panel divider*/
    border-color: rgb(var(--main-accent));
}
.bar-AokMp3 { /*Clicked option container*/
    background: transparent;
}
.emptyChannelIcon-cc932w { /*Empty channel icon*/
    background-color: transparent;
}
.uploadModal-2ifh8j { /*Upload file modal*/
    box-shadow: unset!important;
    background-color: transparent!important;
    border-radius: var(--general-radius);
}
.uploadModal-2ifh8j::before { /*Upload file modal*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.25);
}
.uploadModal-2ifh8j .footer-3mqk7D { /*Upload file modal footer*/
    box-shadow: unset;
    background-color: transparent;
}
.uploadModal-2ifh8j .inner-3nWsbo .file-34mY5K .icon-kyxXVr.image-2yrs5j { /*Upload file preview*/
    background-color: transparent;
}
.wrapper-35wsBm { /*Discord invite embed*/
    background-color: var(--embed-bg);
    border-radius: var(--general-radius)!important;
}
.wrapper-2TxpI8 { /*Video embed*/
    border-radius: var(--general-radius);
    background-color: var(--embed-bg)!important;
}
.iconWrapper-2OrFZ1 .iconBadge-qZ4Ksk { /*New pins color*/
    background-color: rgb(var(--main-accent), 0.85);
}
.channelTextArea-rNsIhG .container-2fRDfG { /*Replying to bar*/
    position: relative;
    background-color: transparent;
    z-index: 1;
}
.cozy-3raOZG .messageContent-2qWWxC { /*Chat message font-size*/
    font-size: var(--message-size);
}
.wrapper-2qzCYF.minimum-28Z35l,
.wrapper-2qzCYF { /*In call background*/
    background-color: transparent;
}
.card-3RzMcx,
.card-3RzMcx:hover { /*New channel cards*/
    background-color: transparent;
}
.messageAttachment-1aDidq { /*Text attachment*/
    max-width: 100%;
    min-width: 0;
}
.tileHorizontal-3eee4N { /*Nitro gift embed*/
    background-color: var(--embed-bg)!important;
    box-shadow: unset!important;
    border-radius: var(--general-radius);
}
.invalidPoopHorizontal-3Dfy7T { /*Nitro gift embed 2*/
    background-color: transparent!important;
}
.attachment-33OFj0 { /*Attached file*/
    border-color: transparent;
    background-color: var(--embed-bg);
    border-radius: var(--general-radius);
}
.wrapperAudio-1jDe0Q { /*Attached audio*/
    border-color: transparent!important;
    background-color: var(--embed-bg)!important;
    border-radius: var(--general-radius)!important;
}
.message-2qRu38 { /*Deleting file*/
    background-color: transparent!important;
}
.role-1P70N6,
.role-1P70N6:hover { /*Allowed roles in channel*/
    background-color: transparent;
}
.operations-36ENbA > a { /*Cancel/save buttons when editing*/
    color: rgba(var(--main-accent), 0.75);
}
.modalTextContainer-ITvzbi { /*Expanded text file*/
    background-color: transparent;
    border-color: transparent;
}
.resultsBlocked-3a77lQ { /*Blocked users results*/
    background-color: transparent;
    border-color: transparent;
}
.invite-18yqGF { /*Spotify invite panel*/
    border-color: transparent!important;
    background-color: transparent!important;
}
.container-1ov-mD > iframe[class="embedSpotify-tvxDCr embedWrapper-lXpS3L"] { /*Spotify embed border*/
    border-radius: 8px!important;
}
.avatar-1BDn8e { /*Chat avatar*/
    padding-left: 0px;
    margin-left: -3px;
}
.content-s2SEQO a,
.wrapper-3WhCwL { /*Description modal links*/
    color: var(--text-link);
}
.content-s2SEQO .wrapper-3WhCwL { /*Description modal channel link*/
    background-color: transparent;
}

/*Code and text preview modals*/

.markup-2BOw-j code { /*Code main modal*/
    background: rgba(0,0,0,0.65);
    border-radius: var(--general-radius);
    border: none;
}
.markup-2BOw-j code.inline {
    background-color: rgba(var(--main-color), 0.5);
    border-radius: var(--general-radius);
}
.container-1pMiXm { /*Text modal main*/
    box-shadow: 0px 0px 2px 1px rgba(var(--main-accent), 0.25);
    border-radius: var(--general-radius);
}
.textContainer-C0szpm { /*Text modal header*/
    background: rgba(0,0,0,0.65 );
    border-radius: var(--general-radius);
    border-bottom-right-radius: 0px;
    border-bottom-left-radius: 0px;
    border: none;
}
.footer-2yA7Ep { /*Text modal footer*/
    background: rgba(0,0,0,0.65 );
    border-radius: var(--general-radius);
    border-top-right-radius: 0px;
    border-top-left-radius: 0px;
    border: none;
}
.hljs-comment, .hljs-quote { /*Code comment/quote*/
    color: green;
}

/*Right click and other popups*/

@keyframes menuAnimation1 {
    0% {
        transform: scaleY(0);
    }
    100% {
        transform: scaleY(1);
    }
}

.menu-3sdvDG { /*Main modal*/
    background-color: transparent;
    border-radius: var(--general-radius);
    animation: menuAnimation1 0.2s ease-in;
    transform-origin: top;
}
.menu-3sdvDG::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    background: var(--menu-bg) no-repeat;
    background-position: center;
    background-size: contain;
    background-color: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.15);
    box-shadow: 0px 0px 4px 2px rgb(var(--main-accent), 0.85);
}
.menu-3sdvDG .scroller-3BxosC { /*Main container*/
    padding-left: 0px;
}
.separator-2I32lJ { /*Separator in menu*/
    border-color: transparent;
}
.scroller-3BxosC .item-1tOPte.labelContainer-1BLJti { /*Main subcontainer text*/
    padding-bottom: 2px;
}
.scroller-3BxosC .item-1tOPte { /*Category in menu*/
    background-color: transparent!important;
    border-color: transparent;
    margin: 0px;
    padding-left: 5px;
    transition: padding-left 0.25s ease-in;
}
.scroller-3BxosC .colorDefault-2K3EoJ:not(.colorDanger-2qLCe1)::after { /*Category in menu underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: transparent;
    border-color: transparent;
    padding-left: 5px;
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.scroller-3BxosC .colorDefault-2K3EoJ.focused-3afm-j { /*Hovered category*/
    background-color: transparent;
    padding-left: 15px;
    transition: 0.25s ease-in;
}
.scroller-3BxosC .colorDefault-2K3EoJ:not(.colorDanger-2qLCe1).focused-3afm-j::after { /*Hovered category underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: rgb(var(--main-accent));
    border-color: transparent;
    transform: translateX(7%);
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.65);
}
.scroller-3BxosC .colorDanger-2qLCe1.focused-3afm-j { /*Leave server button*/
    background-color: transparent;
    color: rgb(240, 71, 71);
}
.scroller-3BxosC .colorDanger-2qLCe1::after { /*Leave server button*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: transparent;
    border-color: transparent;
    padding-left: 5px;
    box-shadow: 0px 0px 0px 0px rgb(240, 71, 71);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.scroller-3BxosC .colorDanger-2qLCe1.focused-3afm-j::after { /*Leave server button hovered*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: rgb(240, 71, 71);
    border-color: transparent;
    transform: translateX(7%);
    box-shadow: 0px 0px 3px 1px rgb(240, 71, 71);
    transition: 0.25s ease-in;
    filter: brightness(0.65);
}

/*Emoji related*/

.emojiSection-3Fb9ix,
.emojiPicker-3PwZFl,
.guildSection-1EoFKd { /*Clicked emoji in chat*/
    background-color: transparent;
}
.emojiSection-3Fb9ix::before { /*Clicked emoji in chat background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    box-shadow: 0px 0px 3px 3px inset rgb(var(--main-accent));
    filter: brightness(0.3);
    width: 100%;
    z-index: -1;
}
.contentWrapper-SvZHNd,
.emojiPicker-3PwZFl { /*Main modal*/
    background-color: transparent;
    border-radius: var(--general-radius);
    box-shadow: unset;
}
.contentWrapper-SvZHNd::before,
.wrapper-1-Fsb8::before,
.premiumPromo-fVlLu-::before,
.diversitySelectorOptions-4YM-vX::before,
.emojiPicker-3PwZFl::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.25);
    z-index: -1;
}
.guildIcon-3h-1IH { /*Emoji server icon*/
    background-color: transparent;
}
.diversitySelectorOptions-4YM-vX { /*Diversity selector*/
    border-radius: var(--general-radius);
    border-color: rgb(var(--main-accent), 0.55);
    background-color: transparent;
}
.diversitySelectorOptions-4YM-vX::before { /*Diversity selector border*/
    border-color: rgb(var(--main-accent), 0.55);
}
.diversityEmojiItem-L6_IXw:hover { /*Diversity selector hovered*/
    background-color: rgba(var(--main-color), .5);
}
.header-8ilj5e { /*Header container*/
    box-shadow: unset;
}
.wrapper-1-Fsb8,
.inspector-S2gM3e { /*Body subcontainers*/
    background-color: transparent;
}
.categoryItemDefaultCategorySelected-_HCKoz,
.categoryItemDefaultCategorySelected-_HCKoz:hover,
.categoryItemDefaultCategory-aBZ6nJ:hover { /*Selected & hovered category*/
    background-color: transparent;
}
.categoryItemDefaultCategory-aBZ6nJ .categoryIcon-1SvUHG {
    filter: brightness(0.3);
}
.categoryItemDefaultCategory-aBZ6nJ:hover .categoryIcon-1SvUHG { /*Hovered category*/
    filter: brightness(1);
    color: rgba(var(--main-accent), 0.35);
    transition: 0.25s ease;
}
.categoryItemDefaultCategorySelected-_HCKoz .categoryIcon-1SvUHG,
.categoryItemDefaultCategorySelected-_HCKoz:hover .categoryIcon-1SvUHG { /*Selected hovered category icon*/
    filter: brightness(1);
    color: rgba(var(--main-accent), 0.85);
    transition: 0.25s ease;
}
.guildCategorySeparator-_An-MP { /*Category divider*/
    border-color: transparent;
}
.emojiItem-14v6tW.emojiItemSelected-1aLkfV { /*Hovered emoji*/
    background-color: rgb(var(--main-accent), 0.35);
}
.header-19cWci[aria-expanded="false"] { /*Emoji category*/
    color: rgb(var(--main-accent), 0.35);
    transition: color 0.25s ease;
}
.header-19cWci[aria-expanded="false"]:hover { /*Hovered emoji category*/
    color: rgb(var(--main-accent), 0.65);
    transition: color 0.25s ease;
}
.header-19cWci[aria-expanded="true"] { /*Selected emoji category*/
    color: rgb(var(--main-accent), 1);
    transition: color 0.25s ease;
}
.header-19cWci.interactive-BzuinF:hover:hover { /*Hovered emoji category*/
    color: rgb(var(--main-accent), 1);
}
.navButtonActive-1MkytQ,
.navButtonActive-1MkytQ:hover { /*Selected GIF/Emoji*/
    background-color: transparent;
    color: rgb(var(--main-accent), 0.85);
    transition: color 0.25s ease;
}
.navButton-2gQCx-:not(.navButtonActive-1MkytQ):hover { /*Hovered GIF/Emoji*/
    color: rgb(var(--main-accent), 0.35);
    transition: color 0.25s ease;
}
.container-2XeR5Z { /*Emoji searchbar*/
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), 0.35);
}
.premiumPromo-fVlLu- { /*Emoji nitro panel*/
    background-color: transparent;
}
.popoutContainer-1MXdqN { /*Clicked emoji modal*/
    background-color: transparent;
}

/*Reactions*/

.reaction-1hd86g { /*Reactions main modal*/
    border: none;
    background: rgba(var(--main-color), 0.5);
    border-radius: var(--general-radius);
    color: white;
}
.reaction-1hd86g.reactionMe-wv5HKu { /*Self reacted*/
    border: none;
    background: rgba(var(--main-accent), 0.15);
    border-radius: var(--general-radius);
}
.reaction-1hd86g:hover { /*Reaction hover*/
    border: none;
    background: rgba(var(--main-accent), 0.05);
}
.button-F9qN4n,
.button-F9qN4n:hover { /*Add reaction*/
    background-color: transparent;
}

/*Guilds*/

@keyframes serverHover { /*Hovered server animation*/
    0% {
        transform: rotate(90deg) scale(0.85);
    }
    100% {
        transform: rotate(90deg) scale(1);
    }
}
@keyframes serverUnHover { /*Hovered server animation*/
    0% {
        transform: rotate(90deg) scale(1);
        box-shadow: 0px 0px 5px 3px rgb(var(--main-accent));
    }
    100% {
        transform: rotate(90deg) scale(0.85);
        box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    }
}

.childWrapper-anI2G9,
.wrapper-1BJsBx.selected-bZ3Lue .childWrapper-anI2G9,
.wrapper-1BJsBx:hover .childWrapper-anI2G9 { /*Home icon background color*/
    background: transparent;
}
.homeIcon-FuNwkv { /*Changes the home icon*/
    color: transparent !important;
    background: url(https://i.imgur.com/Im6DPsl.png) center no-repeat;
    background-size: 45px;
    z-index: 2;
    width: 56px;
    height: 56px;
}
.wrapper-3NnKdC { /*Guild wrapper*/
    border-top-left-radius: var(--general-radius);
    border-top-right-radius: var(--general-radius);
    background: transparent;
    border: 1px solid;
    border-color: rgba(var(--main-accent), 0.3);
    border-bottom-color: transparent;
}
.wrapper-3NnKdC:hover { /*Guild wrapper hover*/
    border-color: rgba(var(--main-accent), 1);
    border-bottom-color: transparent;
}
.wrapper-3NnKdC::before { /*Guild wrapper background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgb(var(--main-color));
    filter: brightness(0.2);
    width: 100%;
}
.tree-2wKJdG, .scroller-1Bvpku { /*Guild subcontainer*/
    background: transparent;
}
.item-2hkk8m { /*Selected server*/
    background-color: rgb(var(--main-accent));
    border-radius: var(--general-radius);
}
.wrapper-25eVIn { /*Guild servers*/
    border-radius: var(--avatar-radius);
    animation: serverUnHover 0.25s ease-in-out;
    animation-fill-mode: forwards;
}
.listItem-GuPuDH:hover .wrapper-25eVIn { /*Hovered server*/
    border-radius: var(--avatar-radius);
    box-shadow: 0px 0px 5px 3px rgb(var(--main-accent));
    animation: serverHover 0.25s ease-in-out;
    animation-fill-mode: forwards;
}
.folderIconWrapper-1_bOZe { /*Collapsed folder background*/
    background-color: transparent!important;
}
.folder-1hbNCn,
.folder-1hbNCn.hover-qTxTR_ { /*Folder background*/
    background-color: transparent;
}
.expandedFolderBackground-1cujaW.collapsed-2ZrjoL { /*Colapsed folder*/
    border-color: transparent;
}
.expandedFolderBackground-1cujaW { /*Expanded folder*/
    border-radius: var(--general-radius);
    background-color: transparent;
    border: 1px solid;
    border-color: rgb(var(--main-accent), 1);
    transition: border-color 0.25s ease;
}
.circleIconButton-1QV--U,
.circleIconButton-1QV--U.selected-1JjBPm { /*Create server & Explore servers*/
    background-color: transparent;
    color: rgba(var(--main-accent), 0.85);
}
.unreadMentionsIndicatorTop-2-tcdU .mention-1f5kbO { /*New messages*/
    background-color: rgb(var(--main-accent), 0.85);
}
.lowerBadge-29hYVK .numberBadge-2s8kKX,
.iconBadge-3qSJIw.participating-1NvRVd { /*Server badges*/
    background-color: transparent!important;
    border-radius: var(--avatar-radius);
}
.lowerBadge-29hYVK .numberBadge-2s8kKX::before,
.iconBadge-3qSJIw.participating-1NvRVd::before { /*Server badges*/
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    border-radius: var(--avatar-radius);
    background-color: rgb(var(--main-accent));
    filter: brightness(0.5);
    z-index: -1;
}
.tree-2wKJdG:focus { /*Removes outline when double clicking guild bar*/
    outline: none;
}

/*Friends window*/

.container-1D34oG { /*Friends and active now panel*/
    background-color: transparent;
}
.title-30qZAO { /*Friends category title (Online, etc...)*/
    text-align: center;
}

@keyframes dmSelected {
    0% {
        filter: brightness(0.25);
    }
    100% {
        filter: brightness(1);
    }
}
.channel-2QD9_O.clickable-1JJAn8.container-2Pjhx-,
.channel-2QD9_O.clickable-1JJAn8.container-2Pjhx- .muted-3mU76i { /*Default DM channel container*/
    transform: translateX(0px);
    transition:  0.25s ease-in;
}
.channel-2QD9_O.clickable-1JJAn8:hover .layout-2DM8Md { /*Hovered DM panel subcontainer*/
    background-color: transparent;
}
.channel-2QD9_O.clickable-1JJAn8.container-2Pjhx-:hover,
.channel-2QD9_O.clickable-1JJAn8.container-2Pjhx-:hover .muted-3mU76i { /*Hovered DM panel container*/
    transform: translateX(8px);
    transition:  0.25s ease-in;
}
.channel-2QD9_O.selected-aXhQR6.container-2Pjhx- { /*Selected DM panel*/
    background-color: transparent;
    transform: translateX(8px);
}
.content-3YMskv .channel-2QD9_O .layout-2DM8Md::after,
.channel-2QD9_O.clickable-1JJAn8.container-2Pjhx-::after,
.channel-2QD9_O.clickable-1JJAn8.container-2Pjhx- .muted-3mU76i::after { /*DM panel*/
    content: '';
    position: absolute;
    left: 0;
    bottom: -5%;
    height: 1px;
    width: 63%;
    background: transparent;
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transform: translateX(0%);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.content-3YMskv .channel-2QD9_O:not(.selected-aXhQR6) .layout-2DM8Md:hover::after { /*Hovered DM*/
    content: '';
    position: absolute;
    left: 0;
    bottom: -5%;
    height: 1px;
    width: 63%;
    background: rgb(var(--main-accent));
    border-color: transparent;
    transform: translateX(37%);
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.channel-2QD9_O.selected-aXhQR6.container-2Pjhx-::after,
.channel-2QD9_O.selected-aXhQR6 .layout-2DM8Md::after { /*Selected DM panel*/
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    height: 1px;
    width: 63%;
    transform: translateX(37%);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent)); 
    animation: dmSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.channel-2QD9_O.selected-aXhQR6 .layout-2DM8Md { /*Selected DM background*/
    background-color: transparent;
}
.peopleList-3c4jOR .title-30qZAO { /*Online friends list title*/
    font-size: 85%;
    color: rgba(var(--main-accent), 0.8);
}
.peopleList-3c4jOR .title-30qZAO::after { /*Line after channel category*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 2.8%;
    left: 18%;
    width: 70%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.peopleList-3c4jOR .title-30qZAO::before { /*Line after channel category 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 3.3%;
    left: 19.35%;
    width: 70%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.tabBody-3YRQ8W:before { /*Annoying line before friends list*/
    box-shadow: unset;
}
.peopleListItem-2nzedh { /*Online friends list*/
    transform: translateY(25%);
    border-top: unset;
}

@keyframes friendSelected { /*Selected friend animation*/
    0% {
        filter: brightness(0.55);
    }
    100% {
        filter: brightness(1);
    }
}
.peopleListItem-2nzedh::after { /*Online friends list*/
    content: '';
    position: absolute;
    bottom: 0;
    left: 0%;
    color: white;
    height: 2px;
    width: 100%;
    background: transparent;
    transform: scaleX(0);
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.55);
}
.peopleListItem-2nzedh:hover { /*Hovered friend*/
    background-color: transparent;
}
.peopleListItem-2nzedh:hover:not(.active-rhSpJJ)::after { /*Hovered friend underline*/
    content: '';
    position: absolute;
    bottom: 0;
    left: 0%;
    color: white;
    height: 2px;
    width: 100%;
    transform: scaleX(1);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 2px rgb(var(--main-accent));
    filter: brightness(0.55);
}
.peopleListItem-2nzedh.active-rhSpJJ { /*Selected friend*/
    background-color: transparent;
}
.peopleListItem-2nzedh.active-rhSpJJ::after { /*Selected friend underline*/
    content: '';
    position: absolute;
    bottom: 0;
    left: 0%;
    color: white;
    height: 2px;
    width: 100%;
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 2px rgb(var(--main-accent));
    animation: friendSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.actionButton-uPB8Fs,
.peopleListItem-2nzedh:hover .actionButton-uPB8Fs,
.actionButton-uPB8Fs.highlight-Lf97TE { /*DM/More options on friend*/
    background-color: transparent;
}
.children-gzQq2t .numberBadge-2s8kKX,
.tabBar-ZmDY9v .badge-1Skb69 { /*Notification*/
    background-color: rgb(var(--main-accent), 0.55)!important;
    border-radius: var(--avatar-radius);
}
.topPill-30KHOu .themed-OHr7kt.selected-3s45Ha.item-PXvHYJ { /*Selected Friends tab*/
    color: rgba(var(--main-accent), 1);
    background-color: transparent!important;
    transition: color 0.25s ease;
}
.topPill-30KHOu .themed-OHr7kt.item-PXvHYJ:hover:not(.disabled-1Hwwfb):not(.selected-3s45Ha) { /*Hovered Friends tab*/
    background-color: transparent;
    color: rgba(var(--main-accent), 0.5);
    transition: color 0.25s ease;
}
.topPill-30KHOu .item-PXvHYJ[aria-controls="ADD_FRIEND-tab"] { /*Add friend tab*/
    color: var(--interactive-normal)!important;
    background-color: transparent!important;
    transition: color 0.25s ease;
}
.topPill-30KHOu .item-PXvHYJ[aria-controls="ADD_FRIEND-tab"]:hover { /*Add friend tab hovered */
    color: rgba(var(--main-accent), 0.5)!important;
    background-color: transparent!important;
    transition: color 0.25s ease;
}
.topPill-30KHOu .item-PXvHYJ[aria-controls="ADD_FRIEND-tab"][aria-selected="true"] { /*Add friend tab selected*/
    color: rgba(var(--main-accent), 1)!important;
}
.sectionHeader-20RGqu { /*Add friends window line*/
    border-color: transparent!important;
}
.wrapper-1cBijl { /*Add friend username input*/
    border-radius: var(--general-radius);
    border-color: rgba(var(--main-color), 0.3);
    transition: border-color 0.25s ease;
}
.wrapper-1cBijl:hover { /*Add friend username input hovered*/
    border-color: rgba(var(--main-accent), 0.35);
    transition: border-color 0.25s ease;
}
.wrapper-1cBijl:focus-within { /*Add friend username input focused*/
    border-color: rgba(var(--main-accent), 1);
}
.quickswitcher-3JagVE { /*Ctrl+K main modal*/
    border-radius: var(--general-radius);
    background-color: transparent;
    box-shadow: none;
}
.quickswitcher-3JagVE::before { /*Ctrl+K main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    box-shadow: 0px 0px 3px 2px rgb(var(--main-accent));
    background-color: rgb(var(--main-color));
    filter: brightness(0.3);
}
.scroller-zPkAnE { /*Ctrl+K body*/
    background-color: transparent;
}
.protip-1b9XPC { /*Ctrl+K protip*/
    border-color: transparent;
}
.quickswitcher-3JagVE .input-2VB9rf { /*Input box*/
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), 0.5);
}
.resultFocused-3aIoYe { /*Result focused*/
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), 0.5);
}
.scroller-9moviB { /*Nitro panel*/
    background-color: transparent;
}
.marketingRefreshSectionTier1-dRwS-6 { /*Dvider*/
    border-color: transparent;
}
.premiumContainer-2Iux5m { /*Nitro window*/
    padding-top: 0px;
}
.hero-EvfTTA { /*Nitro window header*/
    height: 300px;
}

/*Active now*/

.nowPlayingColumn-2sl4cE { /*Main modal*/
    background: transparent;
}
.emptyCard-1RJw8n { /*No active friends modal*/
    background-color: transparent;
    transform: translateY(25%);
}
.scroller-2ZPeAD { /*Active now container*/
    border: none;
    height: 100%;
}
.scroller-2ZPeAD:hover { /*Active now container hover*/
    background-color: transparent!important;
}
.scroller-2ZPeAD .header-13Cw0- { /*Active now text*/
    text-align: center;
    font-size: 85%;
    color: rgba(var(--main-accent), 0.8);
}
.scroller-2ZPeAD .header-13Cw0-::after { /*Line after channel category*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 27px;
    left: 5%;
    width: 75%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.scroller-2ZPeAD .header-13Cw0-::before { /*Line after channel category 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 32px;
    left: 10%;
    width: 75%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.itemCard-v9viV7 { /*Active friends*/
    transform: translateY(25px);
    border-radius: var(--general-radius);
}
.nowPlayingColumn-2sl4cE .wrapper-3D2qGf::after { /*Active friends*/
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    color: white;
    height: 1px;
    width: 100%;
    background: transparent;
    transform: scaleX(0);
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.55);
}
.nowPlayingColumn-2sl4cE .wrapper-3D2qGf { /*Active now card*/
    background-color: transparent;
    border-radius: var(--general-radius);
    border: none;
}
.outer-1AjyKL.interactive-3B9GmY:hover { /*Hovered active now card*/
    background-color: transparent!important;
}
.nowPlayingColumn-2sl4cE .wrapper-3D2qGf:hover:not(.active-1xchHY)::after { /*Hovered active now card underline*/
    content: '';
    position: absolute;
    bottom: 0%;
    left: 0;
    color: white;
    height: 1px;
    width: 100%;
    transform: scaleX(1);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 4px 1px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.55);
}
.outer-1AjyKL.active-1xchHY { /*Selected active now card*/
    background-color: transparent!important;
}
.outer-1AjyKL.active-1xchHY::after { /*Selected active now card underline*/
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    color: white;
    height: 1px;
    width: 100%;
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 4px 1px rgb(var(--main-accent));
    animation: friendSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.inset-3sAvek { /*Active card inner modal*/
    background-color: transparent!important;
    border-radius: var(--general-radius)!important;
    width: 75%;
    transform: translateX(16.5%);
}
.section-2gLsgF { /*User activity container*/
    margin-bottom: 3px;
}
.section-2gLsgF::before { /*User activity container background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-accent), 0.1);
    filter: brightness(1);
    z-index: -1;
}
.separator-XqIyoz { /*Divider*/
    background-color: transparent!important;
}
.partyMemberOverflow-lXnzvu { /*Members in a server*/
    background-color: transparent!important;
}
.container-lRFx4q,
.section-2gLsgF { /*New classes background*/
    background-color: transparent;
}

/*Explore servers*/

.pageWrapper-1PgVDX { /*Main modal*/
    background-color: transparent!important;
    height: 98%;
}
.pageWrapper-1PgVDX::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgb(var(--main-color));
    filter: brightness(0.25);
}
.headerImage-3X1tyY { /*Explore servers banner*/
    display: none;
}
.searchBox-3Y2Vi7 { /*Explore servers searchbar*/
    background-color: transparent!important;
    box-shadow: unset!important;
}
.searchBox-3Y2Vi7::before { /*Explore servers searchbar background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.45);
    z-index: -1;
}
.search-1iTphC .searchBox-2_mAlO,
.input--jS-j2 { /*Explore servers searchbar subcontainer*/
    background-color: transparent;
}

@keyframes searchbarHover {
    0% {
        box-shadow: 0px 0px 0px 0px inset rgb(var(--main-accent));
        filter: brightness(0.35);
    }
    100% {
        box-shadow: 0px 0px 3px 3px inset rgb(var(--main-accent));
        filter: brightness(0.35);
    }
}
@keyframes searchbarUnhover {
    0% {
        box-shadow: 0px 0px 3px 3px inset rgb(var(--main-accent));
        filter: brightness(0.35);
    }
    100% {
        box-shadow: 0px 0px 0px 0px inset rgb(var(--main-accent));
        filter: brightness(0.35);
    }
}
@keyframes searchbarFocus {
    0% {
        box-shadow: 0px 0px 3px 3px inset rgb(var(--main-accent));
        filter: brightness(0.35);
    }
    100% {
        box-shadow: 0px 0px 3px 3px inset rgb(var(--main-accent));
        filter: brightness(1);
    }
}

.searchBoxInputWrapper-nKncfu::after { /*Explore servers searchbar glow*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: var(--main-accent);
    z-index: -1;
    animation: searchbarUnhover 0.25s ease;
    animation-fill-mode: forwards;
}
.searchBoxInputWrapper-nKncfu:hover::after { /*Explore servers searchbar hovered glow*/
    background-color: var(--main-accent);
    filter: brightness(0.35);
    animation: searchbarHover 0.25s ease;
    animation-fill-mode: forwards;
    z-index: -1;
}
.search-1iTphC .searchBox-2_mAlO:focus-within::after { /*Explore servers searchbar focused glow*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: var(--main-accent);
    animation: searchbarFocus 0.25s ease;
    animation-fill-mode: forwards;
}
.search-1iTphC .searchBox-2_mAlO .searchBoxInput-K6mkng,
.search-1iTphC .searchBox-2_mAlO .closeIcon-2WLZc1 { /*Input text and close button*/
    color: rgba(255, 255, 255, 0.685);
}
.card-3DjzTQ { /*Public servers card*/
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), 0.35)!important;
}
.iconMask-3b8GzQ { /*Public servers icon*/
    background-color: transparent!important;
}
.categoryItem-1QIroW:not(.selected-aXhQR6) { /*Category main container*/
    transform: translateX(0px);
    transition:  0.25s ease-in;
}
.categoryItem-1QIroW:not(.selected-aXhQR6)::after { /*Category main container underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 74%;
    background: transparent;
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transform: translateX(0%);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.categoryItem-1QIroW:not(.selectedCategoryItem-FHKU_o):hover { /*Category main container hovered*/
    transform: translateX(12px);
    transition:  0.25s ease-in;
}
.categoryItem-1QIroW:not(.selectedCategoryItem-FHKU_o):hover::after { /*Category main container hovered underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 74%;
    background: rgb(var(--main-accent));
    border-color: transparent;
    transform: translateX(30%);
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.categoryItem-1QIroW.selectedCategoryItem-FHKU_o { /*Category main container selected*/
    transform: translateX(12px);
}
.categoryItem-1QIroW.selectedCategoryItem-FHKU_o::after { /*Category main container selected underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 83%;
    transform: translateX(26.5%);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent)); 
    animation: memberSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.categoryItem-1QIroW.clickable-1JJAn8:hover .layout-2DM8Md { /*Hovered category*/
    background-color: transparent;
}
.categoryItem-1QIroW.selectedCategoryItem-FHKU_o .itemInner-gPkiWb { /*Selected category*/
    background-color: transparent;
}

/*Create server*/

.templatesList-2E6rTe .container-UC8Ug1,
.optionsList-3UMAjx .container-UC8Ug1 { /*Server templates*/
    background-color: transparent;
    border-color: transparent;
}
.header-3msK0M .title-3w8xhj,
.header-1BLHoL .title-LqAd9K,
.header-287ONi .title-Z_XiOC,
.header-1Xr5FO .title-XLSR78 { /*Create server header color*/
    color: rgba(var(--main-accent), 0.75);
}
.footer-2gL1pp .footerTitle-2CYZch {
    color: rgb(var(--main-accent), 0.55);
}
.templatesList-2E6rTe .container-UC8Ug1 .colorStandard-2KCXvj,
.optionsList-3UMAjx .container-UC8Ug1 .colorStandard-2KCXvj { /*Server templates text*/
    color: rgba(255, 255, 255, 0.6);
    transition: color 0.25s ease;
}
.templatesList-2E6rTe .container-UC8Ug1:hover .colorStandard-2KCXvj,
.optionsList-3UMAjx .container-UC8Ug1:hover .colorStandard-2KCXvj { /*Server templates text*/
    color: white;
}
.backButton-iA7KIs,
.footer-2gL1pp .button-38aScr .contents-18-Yxp { /*Back button*/
    color: rgb(var(--main-accent), 0.25);
    transition: color 0.25s ease;
}
.backButton-iA7KIs:hover,
.footer-2gL1pp .button-38aScr:hover .contents-18-Yxp  { /*Back button hovered*/
    color: rgb(var(--main-accent), 0.85);
}
.footer-2gL1pp .button-38aScr:hover .contents-18-Yxp { /*Back button hovered*/
 background-image: none!important;
}
.content-1LAB8Z .input-cIJ7To { /*Server name input*/
    color: rgba(255, 255, 255, 0.75);
}
.iconContainer-2B0ixr svg circle { /*Upload picture circle*/
    fill: rgb(var(--main-accent), 0.35)!important;
    transition: 0.25s ease;
}
.iconContainer-2B0ixr:hover svg circle  { /*Upload picture circle hovered*/
    fill: rgb(var(--main-accent), 0.65)!important;
}
.input--jS-j2 { /*Join server with link*/
    background-color: transparent;
    border-radius: var(--general-radius);
}
.input--jS-j2 .inputDefault-_djjkz {
    color: rgba(255, 255, 255, 0.2)!important;
}
.content-1LAB8Z .formTitle-aeXUoN {
    color: white;
}
.examplesForm-1PzAn- .sampleLink-2NLvZg {
    color: rgba(255, 255, 255, 0.6);
}

/*Server channels & DMs modal*/

@keyframes channelGlowX {
    0% {
        transform: scaleX(0.2);
    }
    100% {
        transform: scaleX(1);
    }
}

.sidebar-2K8pFh,
.sidebar-2K8pFh .container-3w7J-x,
.privateChannels-1nO12o,
.scroller-1JbKMe { /*Main modals*/
    background: transparent;
}
.sidebar-2K8pFh { /*Server channel list*/
    border-radius: 0px;
}
.sidebar-2K8pFh::before { /*Main modal*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgb(var(--main-color));
    filter: brightness(0.25);
    width: 100%;
}
.panels-j1Uci_ { /*User status*/
    background: transparent;
}
.searchBar-6Kv8R2 { /*DMs searchar main modal*/
    background: transparent;
}
.searchBar-6Kv8R2 .searchBarComponent-32dTOx:hover::after,
.searchBar-6Kv8R2 .searchBarComponent-32dTOx { /*DMs searchbar stuff*/
    background: rgba(var(--main-color), 0.25);
    border-radius: var(--general-radius);
    animation: channelGlowX 0.25s ease;
}
.searchBar-6Kv8R2 .searchBarComponent-32dTOx:hover::after { /*DMs searchbar*/
    content: '';
    position: absolute;
    bottom: 25%;
    left: 5%;
    color: white;
    height: 2px;
    width: 90%;
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 2px rgb(var(--main-accent));
    filter: brightness(0.55);
}
.content-3YMskv .containerDefault-3tr_sE,
.content-3YMskv .containerDragAfter-Zk9oyx,
.content-3YMskv .containerDragBefore-1YqewQ,
.content-3YMskv .containerUserOver-98-yc7 { /*Channel categories*/
    text-align: center;
    padding-top: 0px;
    margin-top: 1.5%;
    margin-bottom: 2%;
}
.content-3YMskv .containerDefault-3tr_sE::after { /*Line after channel category*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 12px;
    left: 35px;
    width: 150px;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.content-3YMskv .containerDefault-3tr_sE::before { /*Line after channel category 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 16px;
    left: 50px;
    width: 150px;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.mainContent-2h-GEV svg { /*Channel categories arrow*/
    visibility: hidden;
}
.content-3YMskv .containerDefault-3tr_sE .container-2ax-kl { /*Channel category names*/
    color: rgb(var(--main-accent));
    filter: brightness(0.85);
}
.children-L002ao .addButton-3bLyEA svg polygon{ /*Add channel to category*/
    fill: rgba(var(--main-accent), 0.85)!important;
}
.mainContent-u_9PKf { /*Channel category padding*/
    padding-bottom: 10px;
}

@keyframes channelSelected {
    0% {
        filter: brightness(0.5);
    }
    100% {
        filter: brightness(1);
    }
}
.wrapper-2jXpOf:not(.modeSelected-346R90) { /*Channel names*/
    background-color: transparent;
    transform: translateX(0px);
    transition: 0.25s ease-in;
}
.wrapper-2jXpOf:not(.modeSelected-346R90)::after { /*Channel names underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 83%;
    background: transparent;
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transform: translateX(0px);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.wrapper-2jXpOf:hover:not(.modeSelected-346R90) { /*Channel names hovered*/
    background-color: transparent;
    transform: translateX(14px);
    transition: 0.25s ease-in;
}
.wrapper-2jXpOf:hover:not(.modeSelected-346R90)::after { /*Channel names hovered underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 83%;
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    transform: translateX(14px);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.wrapper-2jXpOf.modeSelected-346R90 { /*Selected channel*/
    background-color: transparent;
    transform: translateX(14px);
}
.wrapper-2jXpOf.modeSelected-346R90::after { /*Selected channel underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 83%;
    transform: translateX(8%);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent)); 
    animation: channelSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.wrapper-2jXpOf:hover .content-1x5b-n,
.modeSelected-346R90 .content-1x5b-n,
.modeSelected-346R90:hover .content-1x5b-n { /*Hovered channel bg*/
    background-color: transparent;
}
.containerDefault--pIXnN .unread-2lAfLh { /*Unread messages in channel*/
    background-color: transparent;
}
.mainContent-u_9PKf[aria-label*="unread,"] .iconContainer-1BBaeJ::before{ /*Unread messages in channel glow*/
    content: '';
    position: absolute;
    top: 35%;
    left: 40%;
    width: 5px;
    height: 5px;
    background-color: rgba(var(--main-accent), 0.4);
    box-shadow: 0px 0px 10px 3px rgb(var(--main-accent)), 0px 0px 0px 0px inset rgb(var(--main-accent));
}
.clickable-25tGDB .header-2V-4Sw:hover,
.selected-31Nl7x .header-2V-4Sw { /*Server name panel*/
    background-color: transparent;
}
.clickable-25tGDB .header-2V-4Sw .button-1w5pas path:nth-child(2),
.clickable-25tGDB .header-2V-4Sw .button-1w5pas path:last-child {
    transition: 0.25s ease;
}
.clickable-25tGDB .header-2V-4Sw:hover .button-1w5pas path:nth-child(2),
.clickable-25tGDB .header-2V-4Sw:hover .button-1w5pas path:last-child { /*Server name arrow*/
    stroke: rgba(var(--main-accent), 1)!important;
    transition: 0.25s ease;
}
.listDefault-3ir5aS .clickable-1lCRLF:hover .content-1Wq3SX { /*Hovered user in VC*/
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), .25);
}
.container-2dqNWc { /*Channel activity preview*/
    border-radius: var(--general-radius);
    background-color: transparent;
}
.container-2dqNWc::before { /*Channel activity preview background*/
    content: '';
    position: fixed;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.25);
    z-index: -1;
}
.activity-3jdl2U+.activity-3jdl2U { /*Activity dividers*/
    border-color: rgb(var(--main-accent), 1);
}
.audienceVoiceUserIconContainer-29oflP { /*Audience icon*/
    background-color: transparent;
}
.moreUsers-7v8yWY { /*More users in channel*/
    border-radius: 0px;
    padding: 0px;
    background-color: transparent;
}
.users-3kndPl { /*Current users in channel*/
    background-color: rgba(var(--main-color), .5);
}
.total-i6us2n { /*Max users in channel*/
    background-color: rgba(var(--main-accent), 0.25);
}
.total-i6us2n:after { /*Max users in channel 2*/
    border-right-color: rgba(var(--main-accent), 0.35);
    filter: brightness(0.56);
}
.container-1giJp5,
.activityPanel-28dQGo,
.listeningAlong-30wH70 { /*User area dividers*/
    border-color: transparent;
}
.gameWrapper-1jIQAX .badge-1JXQev { /*Activity badge*/
    background-color: transparent;
}
.streamPreview-2-WUWT,
.previewContainer-12UlHl,
.previewHover-1tGzfF { /*Stream preview*/
    background-color: transparent!important;
}
.streamPreview-2-WUWT::before { /*Stream preview background*/
    content: '';
    position: absolute;
    top: 0;
    left: 5%;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.35);
    z-index: -1;
}
.avatarSpeaking-2c8-9i { /*Avatar speaking circle*/
    box-shadow: unset;
}
.unreadTop-3rAB3r .unread-1xRYoj,
.unreadBottom-1_LF_w .unread-1xRYoj { /*New undread messages*/
    background-color: transparent;
    border: 1px solid rgb(var(--main-accent), 0.55);
    border-radius: var(--general-radius);
    opacity: 1;
}
.unreadTop-3rAB3r .unread-1xRYoj::before ,
.unreadBottom-1_LF_w .unreadBar-3t3sYc:before { /*New undread messages*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.35);
    z-index: -1;
}
.wrapper-2jXpOf .content-1x5b-n { /*Mentions padding*/
    padding-right: 15px;
}
.children-3rEycc .numberBadge-2s8kKX { /*Channel mentions badge*/
    background-color: transparent!important;
    border-radius: var(--avatar-radius);
}
.children-3rEycc .numberBadge-2s8kKX::before { /*Channel mentions badge background*/
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    border-radius: var(--avatar-radius);
    background-color: rgb(var(--main-accent));
    filter: brightness(0.5);
    z-index: -1;
}

/*Pinned messages*/

.messagesPopoutWrap-1MQ1bW { /*Main modal*/
    background-color: transparent;
    border-radius: var(--general-radius);
    box-shadow: unset;
}
.messagesPopoutWrap-1MQ1bW::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.25);
    z-index: -1;
}
.header-ykumBX { /*Header modal*/
    background-color: transparent;
    box-shadow: unset;
}
.footer-1kmXd4 { /*Footer modal*/
    background-color: transparent;
}
.messageGroupWrapper-o-Zw7G { /*Messages modal*/
    background-color: transparent;
    border-color: rgba(var(--main-color), 0.35);
    border-radius: var(--general-radius);
    transition: border-color 0.25s ease;
}
.messageGroupWrapper-o-Zw7G:hover {/*Messages modal hovered*/
    border-color: rgba(var(--main-accent), 0.65);
}
.jumpButton-3DTcS_ { /*Jump to message color*/
    background-color: transparent;
    color: rgba(var(--main-accent), .55);
    transition: color 0.25s ease;
}
.jumpButton-3DTcS_:hover { /*Jump to message hovered color*/
    color: rgba(var(--main-accent), 1);
}

/*Inbox*/

.container-enaOkj { /*Main modal*/
    background-color: transparent;
}
.container-enaOkj::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.25);
    z-index: -1;
}
.container-3iAQ-0 .channelHeader-3Gd2xq,
.container-3iAQ-0 .messageContainer-gbhlwo { /*Subcontainers*/
    background-color: transparent;
}
.container-3iAQ-0 .messageContainer-gbhlwo { /*Mentioned message*/
    background-color: transparent;
    border: 1px solid;
    border-color: rgba(var(--main-color), 0.35);
    border-radius: var(--general-radius);
    transition: border-color 0.25s ease;
}
.container-3iAQ-0 .messageContainer-gbhlwo:hover {/*Messages modal hovered*/
    border-color: rgba(var(--main-accent), 0.65);
}
.jumpButton-2F6EMx { /*Jump to message container*/
    background-color: transparent;
}
.jumpButton-2F6EMx .text-3KVtey { /*Jump to message color*/
    color: rgba(var(--main-accent), .55);
    transition: color 0.25s ease;
}
.jumpButton-2F6EMx:hover .text-3KVtey { /*Jump to message hovered color*/
    color: rgba(var(--main-accent), 1);
}
.icon-1Itzco,
.secondary-dIudih,
.secondary-dIudih:hover,
.secondary-dIudih:hover:not(.disabled-3Njyym),
.tertiary-aMXF0g,
.tertiary-aMXF0g:hover,
.tertiary-aMXF0g:hover:not(.disabled-3Njyym) { /*Icons*/
    background-color: transparent;
}
.secondary-dIudih:hover:not(.disabled-3Njyym),
.tertiary-aMXF0g:hover:not(.disabled-3Njyym) { /*Icons hovered*/
    color: rgba(var(--main-accent), 0.85);
    transition: color 0.25s ease;
}
.tabBar-1kuXvJ .tab-ck0077.active-1MbGPa { /*Selected tab*/
    background-color: transparent!important;
    color: rgba(var(--main-accent), 1)!important;
    transition: color 0.25s ease;
}
.tabBar-1kuXvJ .themed-OHr7kt.item-PXvHYJ:hover { /*Hovered tab*/
    background-color: transparent!important;
    color: rgb(var(--main-accent), 0.65);
    transition: color 0.25s ease;
}

/*Search messages*/

.container-3ayLPN::before,
.searchBar-3dMhjb::before,
.searchBar-1YE5UV::before { /*Main modals background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.25);
    z-index: -1;
}
.searchBar-1YE5UV { /*Searchbar main modal*/
    background-color: transparent;
    border-radius: var(--general-radius);
    border: 1px solid rgb(var(--main-accent), 0.25);
    transition: border-color 0.25s ease;
}
.searchBar-3dMhjb { /*Searchbar animation*/
    background-color: transparent;
    border-radius: var(--general-radius);
    border: 1px solid rgb(var(--main-accent), 0.25);
    transition: border-color 0.25s ease, width 0.25s ease-in;
}
.searchBar-3dMhjb:not([aria-expanded="true"]):hover,
.searchBar-1YE5UV:hover { /*Searchbar hover*/
    border-color: rgb(var(--main-accent), 0.65);
}
.focused-31_ccS .searchBar-3dMhjb { /*Searchbar focused*/
    border-color: rgb(var(--main-accent), 1);
    transition: border-color 0.25s ease, width 0.25s ease-in;
}
.elevationBorderHigh-2WYJ09 { /*Box shadow on main modal*/
    box-shadow: unset!important;
}

@keyframes menuAnimation2 {
    0% {
        transform: scaleX(0) scaleY(0);
    }
    100% {
        transform: scaleX(1) scaleY(1);
    }
}

.container-3ayLPN { /*Main modal*/
    border-radius: var(--general-radius);
    background-color: transparent!important;
    animation: menuAnimation2 0.25s ease-in;
    transform-origin: top right;
}
.option-96V44q.selected-rZcOL- { /*Hovered option*/
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), 0.25)!important;
}
.option-96V44q::after { /*Options gradient*/
    background: linear-gradient(90deg,rgba(var(--main-accent), 0.05), rgba(var(--main-accent), 0.65) 100%)!important;
}
.resultsGroup-r_nuzN:before { /*Divider*/
    border-color: rgb(var(--main-accent), 0.25)!important;
}
.focused-2bY0OD { /*Searching for results*/
    background-color: transparent!important;
}
.queryContainer-RKFJW- { /*Searching for results 2*/
    border-color: transparent!important;
}
.searchResultsWrap-3-pOjs { /*Search results main modal*/
    position: relative;
    right: -75%;
    border-radius: var(--general-radius);
    background-color: transparent;
    z-index: 1;
}
.searchResultsWrap-3-pOjs::before { /*Search results main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.25);
}
.searchHeader-2XoQg7 { /*Search results header*/
    background-color: transparent;
}
.searchResultGroup-1DphGG .channelName-1JRO3C { /*Result chanel name*/
    background-color: transparent;
    color: rgb(var(--main-accent), 0.85);
}
.searchResultGroup-1DphGG .channelName-1JRO3C:hover {
    text-decoration: unset;
}
.searchResultGroup-1DphGG .searchResult-9tQ1uo { /*Result message*/
    background-color: transparent;
}
.container-2j2llN { /*Result message*/
    background-color: transparent;
    border: 1px solid;
    border-color: rgba(var(--main-color), 0.35);
    border-radius: var(--general-radius);
    transition: border-color 0.25s ease;
}
.container-2j2llN:hover { /*Result message hovered*/
    border-color: rgba(var(--main-accent), 0.65);
}
.button-11zvza { /*Jump to message color*/
    background-color: transparent;
    color: rgba(var(--main-accent), .55);
    transition: color 0.25s ease;
}
.button-11zvza:hover { /*Jump to message hovered color*/
    color: rgba(var(--main-accent), 1);
}
.tab-2j5AEF.selected-2LAck8 { /*Selected tab (New, Old, Relevant)*/
    background-color: transparent!important;
    color: rgb(var(--main-accent));
    transition: color 0.25s ease;
}
.tab-2j5AEF:not(.selected-2LAck8):hover { /*Hovered tab*/
    background-color: transparent!important;
    color: rgba(var(--main-accent), 0.35);
    transition: color 0.25s ease;
}

/*Settings Window*/

.layer-3QrUeG.baseLayer-35bLyl { /*Makes it so the background stays/doesn't open a new "window"*/
    opacity: unset!important;
    transform: unset!important;
}
.layer-3QrUeG { /*Settings background*/
    background-color: rgba(0,0,0,0.8);
}
.layers-3iHuyZ > .layer-3QrUeG.stop-animations:first-child > .container-2lgZY8 > .base-3dtUhz > .content-98HsJk,
.layers-3iHuyZ > .layer-3QrUeG.stop-animations:first-child > .container-2lgZY8 > .guilds-1SWlCJ { /*Blurs the background behind the settings window*/
    z-index: 0;
}
.standardSidebarView-3F1I7i { /*Modifies the settings window*/
    -webkit-backface-visibility: hidden;
    -webkit-perspective: 1000;
    -webkit-transform: translate3d(0,0,0);
    -webkit-transform: translateZ(0);
    backface-visibility: hidden;
    perspective: 1000;
    transform: translate3d(0,0,0);
    transform: translateZ(0);
    position: absolute;
    top: 50%!important;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    width: var(--settings-width);
    height: var(--settings-heigth);
    background: transparent;
    border-radius: var(--general-radius);
}
.standardSidebarView-3F1I7i::before { /*Settings window background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: var(--background-image);
    background-size: cover;
    filter: brightness(0.1);
}
.sidebarRegionScroller-3MXcoP,
.contentRegion-3nDuYy,
.contentRegionScroller-26nc1e,
.background-1QDuV2,
.fieldList-21DyL8 { /*Settings window inner modals*/
    background: transparent;
}

@keyframes closeButtonHover {
    0% {
        filter: brightness(0.55);
    }
    100% {
        filter: brightness(1.25);
    }
}
@keyframes closeButtonUnhover {
    0% {
        filter: brightness(1.25);
    }
    100% {
        filter: brightness(0.55);
    }
}

.closeButton-1tv5uR { /*Close button circle*/
    border-color: transparent!important;
}
.container-1sFeqf:hover .closeButton-1tv5uR svg,
.closeButton-1tv5uR:hover svg,
.container-1sFeqf:hover .keybind-KpFkfr,
.close-hZ94c6:hover { /*Hovered close button & ESC text modals*/
    animation: closeButtonHover 0.25s ease;
    animation-fill-mode: forwards;
}
.container-1sFeqf .closeButton-1tv5uR svg,
.closeButton-1tv5uR svg,
.container-1sFeqf .keybind-KpFkfr,
.close-hZ94c6 { /*Close button & ESC text modals*/
    animation: closeButtonUnhover 0.25s ease;
    animation-fill-mode: forwards;
}
.closeButton-1tv5uR svg path,
.close-hZ94c6 svg path { /*Close button icon*/
    fill: rgb(var(--main-accent))!important;
}
.closeButton-1tv5uR:hover { /*Close button hover*/
    background-color: transparent!important;
}
.keybind-KpFkfr { /*Text under close button*/
    color: rgb(var(--main-accent))!important;
}
.closeButton-1tv5uR::before { /*Close button left backdrop*/
    content: '';
    position: fixed;
    top: calc(0% - calc(100% - var(--settings-heigth)));
    left: -40%;
    width: calc(100% - var(--settings-width));
    height: 2000px;
    cursor: pointer;
    pointer-events: inherit;
    transition: 0.25s ease-in;
}
.closeButton-1tv5uR::after { /*Close button right backdrop*/
    content: '';
    position: fixed;
    top: calc(0% - calc(100% - var(--settings-heigth)));
    left: 100%;
    width: calc(100% - var(--settings-width));
    height: 2000px;
    cursor: pointer;
    pointer-events: inherit;
    transition: 0.25s ease-in;
}
.closeButton-1tv5uR:active { /*Makes the window dissapear*/
    transform: none;
}
.container-3auIfb { /*Checked buttons*/
    border-radius: var(--general-radius);
}
.container-3auIfb:not([style*="background-color: rgb(67, 181, 129);"]) { /*Unchecked buttons*/
    border-radius: var(--general-radius);
    background-color: transparent!important;
}
.container-3auIfb:not([style*="background-color: rgb(67, 181, 129);"])::before { /*Unchecked buttons background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color))!important;
    filter: brightness(0.85);
}
.container-3auIfb:not([style*="background-color: rgb(114, 118, 125);"]) { /*Checked buttons color*/
    border-radius: var(--general-radius);
    background-color: transparent!important;
}
.container-3auIfb:not([style*="background-color: rgb(114, 118, 125);"])::before { /*Checked buttons background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-accent))!important;
    filter: brightness(0.4);
}
.container-3auIfb:not([style*="background-color: rgb(114, 118, 125);"]) svg svg path,
.container-3auIfb:not([style*="background-color: rgb(67, 181, 129);"]) svg svg path { /*Checkmark svg*/
    display: none;
}
.side-8zPYf6 .header-2RyJ0Y { /*Settings window section title*/
    text-align: center;
    font-size: 80%;
    color: rgb(var(--main-accent));
    filter: brightness(0.85);
}
.side-8zPYf6 .header-2RyJ0Y:first-child { /*Settings window first section title*/
    padding-top: 6px;
}
.bd-sidebar-header .header-2RyJ0Y { /*BetterDiscord settings header*/
    width: 100%;
}
.bd-sidebar-header .bd-changelog-button { /*BetterDiscord changelog button*/
    transform: translateX(-80%);
}
.side-8zPYf6 .header-2RyJ0Y::before { /*Settings window section title underline 1*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 17px;
    left: 8px;
    width: 75%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.side-8zPYf6 .header-2RyJ0Y::after { /*Settings window section title underline 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 12px;
    left: -7px;
    width: 75%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.side-8zPYf6 .separator-gCa7yv { /*Settings window sections divider 1*/
    margin: 3px 10px;
    margin-bottom: 5px;
}
.separator-gCa7yv { /*Settings window sections divider 2*/
    background-color: transparent;
}

@keyframes sectionSelected {
    0% {
        filter: brightness(0.5);
    }
    100% {
        filter: brightness(1);
    }
}
.side-8zPYf6 .item-PXvHYJ:not(.selected-3s45Ha):not([aria-controls="Discord Nitro-tab"]):not([aria-controls="GUILD_PREMIUM-tab"]) { /*Settings category main container*/
    transform: translateX(0px);
    transition:  0.25s ease-in;
}
.side-8zPYf6 .item-PXvHYJ:not(.selected-3s45Ha):not([aria-controls="Discord Nitro-tab"]):not([aria-controls="GUILD_PREMIUM-tab"]):not([aria-controls='logout-tab']):after { /*Settings category main container underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: transparent;
    box-shadow: 0px 0px 0px 0px rgb(var(--main-accent));
    transform: translateX(0%);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.side-8zPYf6 .item-PXvHYJ[aria-controls='logout-tab']::after { /*Logout container*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: transparent;
    box-shadow: 0px 0px 0px 0px rgb(240, 71, 71);
    transform: translateX(0%);
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.side-8zPYf6 .item-PXvHYJ:not(.selected-3s45Ha):not([aria-controls="Discord Nitro-tab"]):not([aria-controls="GUILD_PREMIUM-tab"]):hover { /*Settings category main container hovered*/
    background-color: transparent;
    transform: translateX(18px);
    transition:  0.25s ease-in;;
}
.side-8zPYf6 .item-PXvHYJ:not(.selected-3s45Ha):not([aria-controls="Discord Nitro-tab"]):not([aria-controls='logout-tab']):not([aria-controls="GUILD_PREMIUM-tab"]):hover::after { /*Settings category main container hovered underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: rgb(var(--main-accent));
    border-color: transparent;
    transform: translateX(3%);
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.side-8zPYf6 .item-PXvHYJ[aria-controls='logout-tab']:hover {
    background-color: transparent!important;
}
.side-8zPYf6 .item-PXvHYJ[aria-controls='logout-tab']:hover::after { /*Settings LogOut container hovered underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: rgb(240, 71, 71);
    border-color: transparent;
    transform: translateX(3%);
    box-shadow: 0px 0px 3px 1px rgb(240, 71, 71);
    transition: 0.25s ease-in;
    filter: brightness(1);
}
.side-8zPYf6 .selected-3s45Ha.item-PXvHYJ:not([aria-controls="Discord Nitro-tab"]):not([aria-controls="GUILD_PREMIUM-tab"]) { /*Settings category selected*/
    transform: translateX(18px);
    background-color: transparent;
}
.side-8zPYf6 .selected-3s45Ha.item-PXvHYJ:not([aria-controls="Discord Nitro-tab"]):not([aria-controls="GUILD_PREMIUM-tab"]):not([aria-controls='logout-tab'])::after { /*Settings category selected underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    transform: translateX(3%);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent)); 
    animation: sectionSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.side-8zPYf6 .item-PXvHYJ[aria-controls="Discord Nitro-tab"]:not([aria-selected="true"]),
.side-8zPYf6 .item-PXvHYJ[aria-controls="GUILD_PREMIUM-tab"]:not([aria-selected="true"]) { /*Discord category main container*/
    color: var(--interactive-normal)!important;
    transform: translateX(0px);
    transition:  0.25s ease-in;
}
.side-8zPYf6 .item-PXvHYJ[aria-controls="Discord Nitro-tab"]:not([aria-selected="true"])::after,
.side-8zPYf6 .item-PXvHYJ[aria-controls="GUILD_PREMIUM-tab"]:not([aria-selected="true"])::after { /*Discord category main container underline*/
    transform: translateX(0px);
    transition:  0.25s ease-in;
}
.side-8zPYf6 .item-PXvHYJ[aria-controls="Discord Nitro-tab"]:not([aria-selected="true"]):hover,
.side-8zPYf6 .item-PXvHYJ[aria-controls="GUILD_PREMIUM-tab"]:not([aria-selected="true"]):hover { /*Discord category main container hovered*/
    color: var(--interactive-hover)!important;
    background-color: transparent!important;
    transform: translateX(18px);
    transition:  0.25s ease-in;
}
.side-8zPYf6 .item-PXvHYJ[aria-controls="Discord Nitro-tab"]:not([aria-selected="true"]):hover::after,
.side-8zPYf6 .item-PXvHYJ[aria-controls="GUILD_PREMIUM-tab"]:not([aria-selected="true"]):hover::after { /*Discord category main container hovered underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    background: rgb(var(--main-accent));
    border-color: transparent;
    transform: translateX(3%);
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    transition: 0.25s ease-in;
    filter: brightness(0.25);
}
.side-8zPYf6 .item-PXvHYJ[aria-controls="Discord Nitro-tab"][aria-selected="true"],
.side-8zPYf6 .item-PXvHYJ[aria-controls="GUILD_PREMIUM-tab"][aria-selected="true"] { /*Discord category selected*/
    color: var(--interactive-active)!important;
    transform: translateX(18px)!important;
    background-color: transparent!important;
}
.side-8zPYf6 .item-PXvHYJ[aria-controls="Discord Nitro-tab"][aria-selected="true"]::after,
.side-8zPYf6 .item-PXvHYJ[aria-controls="GUILD_PREMIUM-tab"][aria-selected="true"]::after { /*Discord category selected underline*/
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    height: 1px;
    width: 100%;
    transform: translateX(3%);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent)); 
    animation: sectionSelected 0.25s ease;
    animation-fill-mode: forwards;
}
.side-8zPYf6 .themed-OHr7kt.item-PXvHYJ:hover:not(.disabled-1Hwwfb) { /*Hovered selected item*/
    background-color: transparent!important;
}
.divider-3573oO { /*Settings divider*/
    border-color: transparent;
}
.item-26Dhrx,
.item-26Dhrx[aria-checked=true] { /*Privacy and safety DM settings*/
    background-color: transparent;
    border-radius: var(--general-radius);
}
.item-26Dhrx:hover:not([aria-checked=true]) { /*Privacy and safety DM settings hovered*/
    background-color: transparent;
}
.radioBar-bMNUI- { /*Privacy and safety DM border*/
    border-color: transparent!important;
}
.cardWrapper-2Min21 { /*Server to boost card*/
    background-color: transparent;
    border-radius: var(--general-radius);
    border: 1px solid rgba(var(--main-color), .5);
    transition: border-color 0.25s ease;
}
.cardWrapper-2Min21:hover { /*Server to boost card hovered*/
    background-color: transparent;
    border-color: rgba(var(--main-accent), 1.5);
    transition: border-color 0.25s ease;
}
.card-3AyPWq:hover { /*server to boost inner card hovered*/
    background-color: transparent;
}
.wrapper-3nSjSv,
.tier-1EY-yj { /*Nitro deal background*/
    background: transparent;
}
.guildsSection-3AvK09 { /*Server boost divider*/
    border-color: transparent;
}
.codeRedemptionRedirect-1wVR4b { /*Redeemed codes*/
    background-color: transparent!important;
    border-color: transparent!important;
}

@keyframes hoveredItem {
    0% {
        filter: brightness(0.35);
    }
    100% {
        filter: brightness(0.65);
    }
}
@keyframes unhoveredItem {
    0% {
        filter: brightness(0.65);
    }
    100% {
        filter: brightness(0.35);
    }
}
@keyframes selectedItem {
    0% {
        filter: brightness(0.65);
    }
    100% {
        filter: brightness(1.2);
    }
}
@keyframes selectedCircle {
    0% {
        color: transparent;
    }
    100% {
        color: rgb(var(--main-accent));
    }
}

.children-rWhLdy div[aria-labelledby] .item-26Dhrx:first-child::before { /*First privacy option*/
    content: '';
    position: absolute;
    top: 10.8%;
    left: 11%;
    height: 1px;
    width: 80%;
    border-radius: var(--general-radius);
    background: rgb(67, 181, 129);
    box-shadow: 0px 0px 3px 1px rgb(67, 181, 129);
    animation: unhoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.children-rWhLdy div[aria-labelledby] .item-26Dhrx:nth-child(2)::before { /*Second privacy option*/
    content: '';
    position: absolute;
    top: 14.5%;
    left: 11%;
    height: 1px;
    width: 80%;
    border-radius: var(--general-radius);
    background: rgb(250, 166, 26);
    box-shadow: 0px 0px 3px 1px rgb(250, 166, 26);
    animation: unhoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.children-rWhLdy div[aria-labelledby] .item-26Dhrx:last-child::before { /*Last privacy option*/
    content: '';
    position: absolute;
    top: 18.2%;
    left: 11%;
    height: 1px;
    width: 80%;
    border-radius: var(--general-radius);
    background: rgb(240, 71, 71);
    box-shadow: 0px 0px 3px 1px rgb(240, 71, 71);
    animation: unhoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.children-rWhLdy div[aria-labelledby] .item-26Dhrx:first-child:hover:not([aria-checked=true])::before,
.children-rWhLdy div[aria-labelledby] .item-26Dhrx:nth-child(2):hover:not([aria-checked=true])::before,
.children-rWhLdy div[aria-labelledby] .item-26Dhrx:last-child:hover:not([aria-checked=true])::before { /*Hovered privacy options*/
    animation: hoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.children-rWhLdy div[aria-labelledby] .item-26Dhrx[aria-checked=true]::before { /*Selected privacy option*/
    animation: selectedItem 0.25s ease;
    animation-fill-mode: forwards;
}
.radioIconForeground-XwlXQN { /*Selected option circle*/
    animation: selectedCircle 0.25s ease;
    animation-fill-mode: forwards;
}
.cardPrimary-1Hv-to { /*Terms and conditions container*/
    background-color: transparent;
    border-color: transparent;
}
.cardPrimaryOutline-29Ujqw { /*Authorized apps container*/
    border-radius: var(--general-radius);
    border-color: rgba(var(--main-color), 0.3);
    transition: border-color 0.25s ease-in;
} 
.cardPrimaryOutline-29Ujqw:hover { /*Authorized apps container hovered*/
    border-radius: var(--general-radius);
    border-color: rgba(var(--main-accent), 0.65);
    transition: border-color 0.25s ease-in;
}
.accountList-33MS45,
.connectionList-3pzR-1 { /*Connections main panels*/
    background: transparent;
    border-radius: var(--general-radius);
}
.connectedAccounts-2-XP1G { /*Connected acounts modal*/
    height: 65px;
}
.wrapper-3JPufy { /*App to connect wrapper*/
    height: 52px;
}
.accountBtn-2Nozo3 { /*App to connect main container*/
    margin-bottom: 0;
    height: 52px;
    top: 15%;
    transition: margin-top 0.25s ease;
}
.accountBtn-2Nozo3:hover { /*App to connect main container hovered*/
    margin-top: -14px;
    height: 58px;
}
.accountBtn-2Nozo3 .accountBtnInner-sj5jLs { /*App to connect subcointainer background*/
    background-color: transparent;
}
.accountBtn-2Nozo3 .accountBtnInner-sj5jLs:hover { /*App to connect subcontainer hovered background*/
    background-color: transparent;
    padding-bottom: 20px;
}
.connection-1fbD7X,
.connectionHeader-2MDqhu { /*Connected accounts*/
    background-color: transparent;
}
.connection-1fbD7X { /*Connected accounts modal*/
    border: 1px solid;
    border-color: rgba(var(--main-color), 0.3);
    transition: border-color 0.25s ease-in;
}
.connection-1fbD7X:hover { /*Connected accounts modal hovered*/
    border-color: rgba(var(--main-accent), 0.65);
    transition: border-color 0.25s ease-in;
}
.connection-1fbD7X .connectionDelete-2Odoln svg path { /*Connected account delete button*/
    fill: rgb(var(--main-color))!important;
    transition: 0.25s ease;
}
.connection-1fbD7X:hover .connectionDelete-2Odoln svg path { /*Connected account delete button panel hovered*/
    fill: rgb(var(--main-accent))!important;
    transition: 0.25s ease;
}
.connectionDelete-2Odoln svg { /*Connected account delete button*/
    animation: closeButtonUnhover 0.25s ease;
    animation-fill-mode: forwards;
}
.connectionDelete-2Odoln:hover svg path { /*Connected account delete button hovered*/
    fill: rgb(var(--main-accent))!important;
}
.connectionDelete-2Odoln:hover svg { /*Connected account delete button hovered*/
    animation: closeButtonHover 0.25s ease;
    animation-fill-mode: forwards;
}
.integration-3kMeY4 { /*Connected sub servers*/
    background-color: transparent;
}
.hero-EvfTTA { /*Discord nitro image*/
    background: url();
}
.feature-2w65J5 { /*Discord nitro features*/
    background-color: transparent!important;
}
.barFill-23-gu- { /*Filled bar color*/
    background: rgba(var(--main-accent), 0.85);
}
.bar-2Qqk5Z {
    background: rgba(var(--main-color), 0.45)!important;
}
.defaultValue-3gC7yw .markValue-2DwdXI { /*Defalt text scale color*/
    color: rgba(var(--main-accent), 0.55);
}
.userSettingsVoice-iwdUCU .media-engine-video { /*Camera preview main modal*/
    background-color: transparent;
}
.userSettingsVoice-iwdUCU .previewOverlay-2O7_KC { /*Camera preview window*/
    background-color: transparent!important;
    border-color: transparent!important;
}
.notches-1sAcEM { /*Test voice bar notches*/
    background-image: url()!important;
}
.progress-1IcQ3A { /*Test voice bar progress background*/
    background-color: rgb(var(--main-color))!important;
    filter: brightness(0.45);
}
.container-3PXSwK { /*Test voice bar progress color*/
    background: linear-gradient(to right, rgba(var(--main-accent), 0.25), rgba(var(--main-accent), 1))!important;
}
.inputSensitivityToggle-2LKb8o .bar-2Qqk5Z { /*Voice sensitivity bar*/
    background: rgba(var(--main-color), 0.45)!important;
}
.inputSensitivityToggle-2LKb8o .barFill-23-gu- { /*Voice sensitivity bar 2*/
    background: rgba(var(--main-accent), 0.85)!important;
}
.row-2okwlC { /*Divider between keybinds*/
    box-shadow: unset!important;
    margin-bottom: 4%;
}
.row-2okwlC .card-FDVird::before { /*Keybind panel*/
    opacity: 1;
    border: 1px solid rgba(var(--main-color), .5);
    background-color: transparent!important;
    border-color: rgba(var(--main-color), .5)!important;
    border-radius: var(--general-radius);
    transition: border-color 0.25s ease;
}
.row-2okwlC .card-FDVird:hover::before { /*Keybind panel hovered*/
    border-color: rgba(var(--main-accent), .65)!important;
    transition: border-color 0.25s ease;
}
.activeGame-14JI7o { /*Active game*/
    background-color: transparent!important;
    border-radius: var(--general-radius);
}
.game-1ipmAa { /*Added games*/
    margin-bottom: 3%;
    box-shadow: unset!important;
}
.game-1ipmAa.card-FDVird::before { /*Added games*/
    opacity: 1;
    border-color: transparent;
    background-color: transparent!important;
    border-radius: var(--general-radius);
    transition: border-color 0.25s ease;
}
.overlayToggleIconOn-3UNmty .fill-1ugeBG { /*Overlay Icon ON*/
    fill: rgba(var(--main-accent), 0.85)!important;
    transition: 0.25s ease;
}
.overlayToggleIcon-2liB3r:hover .overlayToggleIconOn-3UNmty { /*Overlay Icon ON hover*/
    filter: brightness(0.4);
    transition: 0.25s ease;
}
.overlayToggleIcon-2liB3r:hover .overlayToggleIconOn-3UNmty .fill-1ugeBG path{ /*Overlay Icon ON hover 2*/
    fill: #f04747!important;
    transition: 0.25s ease;
}
.overlayToggleIcon-2liB3r:hover .overlayToggleIconOn-3UNmty path {/*Overlay Icon ON hover 3*/
    fill: #f04747!important;
    d: path("M 8.67872 19 H 11 V 21 H 7 V 23 H 17 V 21 H 13 V 19 H 20 C 21.103 19 22 18.104 22 17 V 6 C 22 5.89841 21.9924 5.79857 21.9777 5.70101 L 20 7.67872 V 15 H 12.6787 L 8.67872 19 Z M 13.1496 6 H 4 V 15 H 4.14961 L 2.00515 17.1445 C 2.00174 17.0967 2 17.0486 2 17 V 6 C 2 4.897 2.897 4 4 4 H 15.1496 L 13.1496 6 Z");
    transition: 0.25s ease;
}
.overlayToggleIconOff-1kT42w .fill-1ugeBG,
.overlayToggleIconOff-1kT42w rect { /*Overlay Icon OFF*/
    transition: 0.25s ease;
}
.overlayToggleIcon-2liB3r:hover .overlayToggleIconOff-1kT42w .fill-1ugeBG { /*Overlay Icon OFF hover*/
    fill: rgba(var(--main-accent), 0.4)!important;
    transition: 0.25s ease;
}
.overlayToggleIcon-2liB3r:hover .overlayToggleIconOff-1kT42w path {
    d: path("M 4 2.5 C 2.897 2.5 2 3.397 2 4.5 V 15.5 C 2 16.604 2.897 17.5 4 17.5 H 11 V 19.5 H 7 V 21.5 H 17 V 19.5 H 13 V 17.5 H 20 C 21.103 17.5 22 16.604 22 15.5 V 4.5 C 22 3.397 21.103 2.5 20 2.5 H 4 Z M 20 4.5 V 13.5 H 4 V 4.5 H 20 Z");
    transition: 0.25s ease;
}
.overlayToggleIcon-2liB3r:hover .overlayToggleIconOff-1kT42w rect {
    display: none;
    transition: 0.25s ease;
}
.game-1ipmAa .removeGame-2JFGPn { /*Remove game button*/
    background-color: transparent;
    box-shadow: unset;
    filter: brightness(0.55);
    transition: 0.25s ease;
}
.game-1ipmAa .removeGame-2JFGPn:hover { /*Remove game button hover*/
    background-color: transparent;
    box-shadow: unset;
    filter: brightness(1);
    transition: 0.25s ease;
}
.wrapper-3jrx9n { /*Overlay position*/
    border-radius: 5px;
    border-color: rgba(var(--main-accent), .35);
}
.option-n0icdO { /*Overlay position options*/
    border-radius: 5px;
    background-color: rgba(var(--main-color), .5);
    transition: background-color 0.25s ease;
}
.option-n0icdO:hover { /*Overlay position option hovered*/
    background-color: rgba(var(--main-accent), .35);
    transition: background-color 0.25s ease;
}
.selected-mKYnfr.option-n0icdO { /*Selected overlay position*/
    background-color: rgba(var(--main-accent), .65);
    border-color: rgba(var(--main-accent), .65);
    transition: 0.25s ease;
}
.disabledIcon-9QatvX { /*Disabled overlay option*/
    transition: 0.25s ease;
}
.root-1gCeng,
.footer-2gL1pp { /*Changelog modal*/
    box-shadow: unset!important;
    background-color: transparent!important;
    border-radius: var(--general-radius);
}
.root-1gCeng::before { /*Changelog background color*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.35);
    z-index: -1;
}
.preview-2nSL_2 { /*Discord mode preview*/
    border: none!important;
    background-color: transparent;
}


/*Input devices dropbox*/

.css-gvi9bl-control,
.css-1kj8ui-container,
.bd-select { /*Main input device dropbox*/
    background-color: transparent;
    border-radius: var(--general-radius);
    border-color: rgba(var(--main-color), .5);
    transition: border-color 0.25s ease;
}
.css-17e1tep-control,
.css-17e1tep-control:focus,
.css-17e1tep-control:active { /*Focused main input device dropbox*/
    border-radius: var(--general-radius);
    background-color: transparent;
    border-color: rgba(var(--main-accent), 1.5)!important;
    transition: border-color 0.25s ease;
}
.css-gvi9bl-control:hover,
.bd-select:hover { /*Main input device dropbox hovered*/
    background-color: transparent;
    border-color: rgba(var(--main-accent), 0.3);
    transition: border-color 0.25s ease;
}
.css-6fzn47-control:hover,
.css-6fzn47-control,
.bd-select.menu-open { /*Main input device dropbox selected/focused*/
    border-radius: var(--general-radius) var(--general-radius) 0px 0px;
    border-bottom-color: transparent!important;
    background-color: transparent;
    border-color: rgba(var(--main-accent), 1.5);
    transition: border-color 0.25s ease;
}
.css-1ba14n5-option,
.bd-select .bd-select-option.selected { /*Dropdown menu selected option*/
    background-color: transparent;
    color: rgba(var(--main-accent), 0.85)!important;
}
.css-3vaxre-menu,
.bd-select .bd-select-options { /*Dropdown menu open*/
    border-radius: 0px 0px var(--general-radius) var(--general-radius);
    background-color: transparent;
    border-color: rgba(var(--main-accent), 1.5);
    border-top-color: transparent!important;
    animation: menuAnimation1 0.2s ease-in;
    transform-origin: top;
    transition: border-color 0.25s ease;
}
.css-3vaxre-menu::before,
.bd-select .bd-select-options::before { /*Dropdown menu open background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: 0px 0px var(--general-radius) var(--general-radius);
    background: rgb(var(--main-color));
    filter: brightness(0.25);
    z-index: -1;
}
.css-rzbxvl-option,
.bd-select .bd-select-option:hover { /*Hovered main input option*/
    color: rgba(var(--main-accent), 0.55);
}
.bd-select .bd-select-option:hover { /*Hovered main input option*/
    background-color: transparent;
}

/*General button settings*/

.fieldButton-27bJrp { /*Edit button in settings*/
    border-radius: var(--general-radius);
    background-color: transparent!important;
    transition: 0.25s ease;
}
.fieldButton-27bJrp:hover { /*Edit button in settings hovered*/
    color: rgb(var(--main-accent))!important;
    filter: brightness(1.2);
    transition: 0.25s ease;
}
.lookOutlined-3sRXeN.colorWhite-rEQuAQ,
.button-uXr0L2 { /*Activity buttons*/
    border-radius: var(--general-radius);
    border-color: rgba(var(--main-accent), 0.3);
    transition: border-color 0.25s ease;
}
.lookOutlined-3sRXeN.colorBrand-3pXr91 { /*Request data button*/
    color: white;
}
.lookFilled-1Gx00P.colorRed-1TFJan,
.lookOutlined-3sRXeN.colorRed-1TFJan { /*Delete/disable account buttons*/
    color: white;
    border-radius: var(--general-radius);
    border: 1px solid rgba(240, 71, 71, 0.15);
    background-color: transparent;
    transition: border-color 0.25s ease;
}
.lookFilled-1Gx00P.colorBrand-3pXr91,
.lookOutlined-3sRXeN.colorBrand-3pXr91 { /*Change password/Enable 2FA/Request data buttons*/
    border-radius: var(--general-radius);
    border: 1px solid rgba(var(--main-color), .5);
    background-color: transparent;
    transition: border-color 0.25s ease;
}
.lookOutlined-3sRXeN.colorWhite-rEQuAQ:hover,
.lookFilled-1Gx00P.colorBrand-3pXr91:hover,
.lookOutlined-3sRXeN.colorBrand-3pXr91:hover,
.button-uXr0L2:not([disabled]):hover { /*Activity buttons hovered*/
    border-radius: var(--general-radius);
    border-color: rgba(var(--main-accent), 1.5);
    transition: border-color 0.25s ease;
}
.lookFilled-1Gx00P.colorRed-1TFJan:hover,
.lookOutlined-3sRXeN.colorRed-1TFJan:hover { /*Delete/disable account buttons hover*/
    background-color: transparent;
    border-color: rgba(240, 71, 71, 1.5);
    border-radius: var(--general-radius);
}
.lookFilled-1Gx00P.colorBrand-3pXr91:hover { /*Change password/Enable 2FA/Request data buttons hovered*/
    background-color: transparent;
}
.lookOutlined-3sRXeN.colorWhite-rEQuAQ:disabled,
.lookFilled-1Gx00P.colorBrand-3pXr91:disabled,
.button-uXr0L2[disabled] { /*Activity buttons disabled*/
    border-color: rgba(var(--main-color));
    filter: brightness(0.4);
    transition: border-color 0.25s ease;
}
.lookFilled-1Gx00P.colorBrand-3pXr91:disabled { /*Change password/Enable 2FA/Request data buttons disabled*/
    background-color: transparent;
}
.lookInverted-2D7oAl.colorBrand-3pXr91,
.lookFilled-1Gx00P.colorGreen-29iAKY,
.lookFilled-1Gx00P.colorPrimary-3b3xI6,
.lookInverted-2D7oAl.colorGreen-29iAKY,
.lookFilled-1Gx00P.colorGrey-2DXtkV,
.theme-dark .lookOutlined-3sRXeN.colorPrimary-3b3xI6,
.lookGhost-2Fn_0-.colorGrey-2DXtkV,
.theme-dark .watchButton-2SbJEo  { /*Subscribe/Gift Nitro buttons*/
    color: white;
    background-color: transparent!important;
    border: 1px solid rgba(var(--main-color), .5);
    border-radius: var(--general-radius);
    transition: border-color 0.25s ease;
}
.lookInverted-2D7oAl.colorBrand-3pXr91:hover,
.lookFilled-1Gx00P.colorGreen-29iAKY:hover,
.lookFilled-1Gx00P.colorPrimary-3b3xI6:hover,
.lookInverted-2D7oAl.colorGreen-29iAKY:hover,
.lookFilled-1Gx00P.colorGrey-2DXtkV:hover,
.button-1YfofB.buttonColor-7qQbGO.buttonActive-3FrkXp,
.theme-dark .lookOutlined-3sRXeN.colorPrimary-3b3xI6:hover,
.lookGhost-2Fn_0-.colorGrey-2DXtkV:hover,
.theme-dark .watchButton-2SbJEo:not([disabled]):hover { /*Subscribe/Gift Nitro white buttons hovered*/
    background-color: transparent!important;
    border-color: rgba(var(--main-accent), 1.5);
    transition: border-color 0.25s ease;
}
.lookGhost-2Fn_0-.colorGrey-2DXtkV:hover { /*Copy button hover*/
    color: rgba(255, 255, 255, 0.85);
    transition: color 0.1s ease;
}
.button-2PWmas:hover { /*Notice back button*/
    background-color: transparent;
}
.button-14-BFJ.enabled-2cQ-u7 { /*Mute/Deafen/Config buttons*/
    transition: color 0.25s ease;
}
.button-14-BFJ.enabled-2cQ-u7 .strikethrough-1n4ekb { /*Muted/Deafened cross line*/
    color: rgba(var(--main-accent), 0.85);
}
.button-14-BFJ.enabled-2cQ-u7:hover { /*Mute/Deafen/Config buttons hovered*/
    background-color: transparent;
    color: rgba(var(--main-accent), 0.65);
}
.colorable-1bkp8v.primaryDark-3mSFDl,
.colorable-1bkp8v.primaryDark-3mSFDl:hover { /*Sharing screen buttons*/
    background-color: transparent;
}
.button-3HqqDX { /*Invite people button*/
    background-color: transparent;
}
.button-1YfofB.buttonColor-7qQbGO.fauxDisabled-2ik0Vw,
.button-1YfofB .buttonColor-7qQbGO.fauxDisabled-2ik0Vw,
.button-1YfofB.buttonColor-7qQbGO:disabled,
.button-1YfofB .buttonColor-7qQbGO:disabled { /*Disabled buttons*/
    background-color: transparent;
}
.lookFilled-1Gx00P.colorRed-1TFJan.button-38aScr .contents-18-Yxp,
.lookOutlined-3sRXeN.colorRed-1TFJan.button-38aScr .contents-18-Yxp { /*Delete button*/
    color: rgba(240, 71, 71, 0.5)!important;
    transition: color 0.25s ease;
}
.lookFilled-1Gx00P.colorRed-1TFJan.button-38aScr:hover .contents-18-Yxp,
.lookOutlined-3sRXeN.colorRed-1TFJan.button-38aScr:hover .contents-18-Yxp { /*Delete button hover*/
    color: rgba(240, 71, 71, 1)!important;
    transition: color 0.25s ease;
}

/*Blur Username, E-mail and phone in settings*/

.field-1HUseB+.field-1HUseB .colorHeaderPrimary-26Jzh-.size16-1P40sf { /*Blurs e-mail and phone number*/
    filter: blur(8px);
}
.field-1HUseB+.field-1HUseB .colorHeaderPrimary-26Jzh-.size16-1P40sf:hover { /*Unblurs e-mail and phone number*/
    filter: blur(0px);
    transition: 0.2s ease;
}
.usernameInnerRow-ZlFnET { /*Blurs username*/
    filter: blur(8px);
}
.usernameInnerRow-ZlFnET:hover { /*Unblurs username*/
    filter: blur(0px);
    transition: 0.2s ease;
}

/*BD settings*/

.bd-switch-body { /*BD checkbox default/unchecked*/
    border-radius: var(--general-radius);
    --switch-color: rgb(var(--main-color));
}
.bd-switch-body::before { /*BD checkbox default/unchecked background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-color));
    filter: brightness(0.85);
}
.bd-switch input:checked+.bd-switch-body { /*BD checked checkbox*/
    border-radius: var(--general-radius);
    --switch-color: rgb(var(--main-color));
}
.bd-switch input:checked+.bd-switch-body::before { /*BD checked checkbox background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-accent));
    filter: brightness(0.4);
}
.bd-setting-divider { /*BD settings divider*/
    border-color: transparent;
}
.bd-settings-group.collapsible .bd-settings-title::before,
.bd-settings-group.collapsible .bd-settings-title::after { /*Line after settings section title expanded*/
    background-color: rgb(var(--main-accent));
    filter: brightness(1);
    transition: 0.25s ease-in;
}
.bd-settings-group.collapsed .bd-settings-title::before,
.bd-settings-group.collapsed .bd-settings-title::after { /*Line after settings section title collapsed*/
    background-color: rgb(var(--main-accent));
    filter: brightness(0.35);
    transition: 0.25s ease;
}
.bd-button { /*BD blue buttons*/
    border-radius: var(--general-radius);
    background-color: transparent;
    transition: 0.25s ease;
}
.bd-button:hover { /*BD blue buttons hovered*/
    background-color: transparent;
    color: rgb(var(--main-accent));
    filter: brightness(1.2);
}
.bd-addon-views .bd-view-button.selected { /*BD button selected view*/
    background-color: transparent;
    filter: brightness(1);
    transition: 0.25s ease;
}
.bd-view-button { /*BD view button*/
    filter: brightness(0.2);
    transition: 0.25s ease;
}
.bd-view-button:hover { /*BD view button hovered*/
    background-color: transparent!important;
    filter: brightness(0.5);
    transition: 0.25s ease;
}
.bd-search-wrapper { /*BD searchbar*/
    border: 1px solid rgba(var(--main-color), .5);
    border-radius: var(--general-radius);
    background-color: transparent;
    transition: border-color 0.25s ease;
}
.bd-search-wrapper:hover { /*BD searchbar hovered*/
    border-color: rgba(var(--main-accent), .65);
    transition: border-color 0.25s ease;
}
.bd-addon-list .bd-addon-card { /*BD addon container*/
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), .25);
}
.bd-addon-list .bd-addon-header { /*BD addon container header*/
    background-color: rgba(var(--main-color), 0.15);
}
.bd-changelog-modal code.inline { /*Inline code*/
    background-color: rgba(var(--main-color), 0.65);
}

/*Server boost*/

.root-3R2ngo::before { /*Server boost backdrop*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgb(0,0,0);
    opacity: 0.8;
}
.perksModal-fSYqOq { /*Main modal*/
    top: 50%!important;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    width: var(--settings-width);
    height: var(--settings-heigth);
    background: transparent!important;
    border-radius: var(--general-radius);
    pointer-events: all!important;
}
.perksModal-fSYqOq::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    height: 170%;
    background: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.25);
    z-index: -1;
}
.root-3R2ngo .closeButton-1tv5uR::before { /*Close button left backdrop*/
    content: '';
    position: fixed;
    top: 0;
    left: 0;
    width: calc(80% - var(--settings-width));
    height: 100%;
    cursor: pointer;
    pointer-events: inherit;
    transition: 0.25s ease-in;
}
.root-3R2ngo .closeButton-1tv5uR::after { /*Close button right backdrop*/
    content: '';
    position: fixed;
    top: 0;
    left: calc(20% + var(--settings-width));
    width: calc(80% - var(--settings-width));
    height: 100%;
    cursor: pointer;
    pointer-events: inherit;
    transition: 0.25s ease-in;
}
.root-3R2ngo .closeButton-1tv5uR:active { /*Makes the window dissapear*/
    transform: none;
}
.ctaBar-2UsjF2 { /*Server container*/
    background-color: transparent;
    background-image: url()!important;
}
.container-1sFeqf { /*Close window button*/
    right: -35%;
    top: 80px;
}
.carousel-18mXWH { /*Server level panels*/
    left: 15px!important;
}
.tierWrapper-W9ajqp { /*Server tier wrappers*/
    border-radius: var(--general-radius);
    background-color: transparent;
    box-shadow: unset!important;
}
.tierWrapper-W9ajqp::before { /*Server tier wrappers background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.55);
    z-index: -1;
}
.tierMarkerBackground-3q29am { /*Server boost level progress bar*/
    background-color: transparent!important;
}
.iconWrapper-3LVgIo { /*Server boost quantity*/
    background: transparent!important;
}
.iconWrapper-3LVgIo:hover { /*Server boost quantity hover*/
    background: rgb(var(--main-accent), 0.55)!important;
}
.icon-TYbVk4, .icon-TYbVk4.disabled-24YXy-, .icon-TYbVk4.disabled-24YXy-:hover { /*Server boost quantity*/
    color: white;
}
.tier-12tKuZ { /*Server boost tier container*/
    border-radius: var(--general-radius);
}
.tierBody-16Chc9 { /*Server boost tier card body*/
    background-color: transparent!important;
}
.perk-2WeBWW { /*Server boost perks*/
    background-color: transparent!important;
}
.divider-25_-sM { /*Server boost divider*/
    background-color: transparent;
}
.tierBody-x9kBBp { /*Server boost tier body*/
    background-color: rgba(var(--main-color), 0.25)!important;
}
.tierHeaderLocked-1a2opw { /*Server boost tier header*/
    background-color: rgba(var(--main-color), 0.1)!important;
}
.upsellFooter-3coAfO,
.value-IR9osW  { /*Buying boosts*/
    background-color: transparent;
}

/*Windows bar*/

.withFrame-haYltI::before { /*Windows bar*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgb(var(--main-color))!important;
    filter: brightness(0.25);
    width: 100%;
    height: 2.1%!important;
}
.wordmark-2iDDfm { /*Discord Wordmark*/
    color: transparent;
}
.withFrame-haYltI::after { /*Wordmark*/
    content: "POISON";
    font-family: 'Fjalla One', sans-serif!important;
    position: absolute;
    font-size: 1rem;
    color: rgba(var(--main-accent), 0.5)!important;
    left: 0.8%;
    top: 4px;
}
.winButton-iRh8-Z { /*Windows minimize/maximize*/
    color: rgba(var(--main-accent), 0.35);
    transition: color 0.25s ease;
}
.winButton-iRh8-Z:hover { /*Windows minimize/maximize hover*/
    background-color: transparent;
    color: rgba(var(--main-accent), 0.85);
}
.winButtonClose-1HsbF- { /*Window close button*/
    color: rgba(255, 0, 0, 0.5);
    transition: color 0.25s ease;
}
.winButtonClose-1HsbF-:hover { /*Windows close button hover*/
    color: rgba(255, 0, 0, 1);
}

/*User cards*/

.userPopout-3XzG_A { /*Main modal*/
    box-shadow: unset;
    border-radius: var(--general-radius);
    box-shadow: unset;
}
.userPopout-3XzG_A::before { /*Main modal bg*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.25);
    z-index: -1;
}
.headerTop-3C2Zn0 {
    filter: brightness(0.95);
}
.header-2BwW8b,
.headerPlaying-j0WQBV,
.headerTop-3C2Zn0,
.body-3iLsc4,
.footer-1fjuF6 { /*Body modals*/
    background-color: transparent!important;
}
.barInner-3NDaY_ { /*Spotify progress bar*/
    background-color: rgba(var(--main-accent), 0.85)!important;
}
.activity-11LB_k { /*Activity main modal*/
    filter: brightness(0.9);
}
.activityUserPopout-2yItg2 .headerText-1HLrL7 { /*Activity header text*/
    justify-content: center!important;
    color: rgb(var(--main-accent))!important;
    filter: brightness(0.93);
}
.bodyTitle-Y0qMQz { /*Role/Message title text*/
    text-align: center;
    color: rgb(var(--main-accent))!important;
    filter: brightness(0.75);
    margin-bottom: 7%;
}
.activityUserPopout-2yItg2 .headerText-1HLrL7::after,
.bodyTitle-Y0qMQz::after { /*Line after channel category*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 7px;
    left: 12%;
    width: 150px;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.activityUserPopout-2yItg2 .headerText-1HLrL7::before,
.bodyTitle-Y0qMQz::before { /*Line after channel category 2*/
    content: '';
    position: absolute;
    overflow: hidden!important;
    top: 12px;
    left: 27%;
    width: 100%;
    height: 20px;
    background: radial-gradient(16px, transparent, transparent 4px, rgb(var(--main-accent)) 4px, rgb(var(--main-accent)) 10px, transparent 11px);
    background-position: 0px -20px;
    background-size: 30px 40px;
    transform: scaleY(0.25) scaleX(1.5);
    filter: brightness(0.85);
}
.botTagInvert-18-95s { /*User card bot tag*/
    background-color: rgba(var(--main-accent), 0.35);
    color: white;
}
.input-cIJ7To { /*Message user*/
    border-color: rgba(var(--main-color), .5);
    border-radius: var(--general-radius);
}
.input-cIJ7To:hover { /*Message user hover*/
    border-color: rgba(var(--main-accent), 0.25);
}
.input-cIJ7To:focus { /*Message user focus*/
    border-color: rgba(var(--main-accent), 1);
}
.note-3HfJZ5 { /*User card note*/
    border-radius: var(--general-radius);
    margin-left: 0px;
    margin-right: 0px;
    width: 99.085%;
    height: 50%;
}
.textarea-2r0oV8 { /*User card note text area*/
    width: 100.93%!important;
    height: 50%!important;
    border: 1px solid rgba(var(--main-color), .5);
    border-radius: var(--general-radius);
    background-color: transparent!important;
}
.headerNormal-T_seeN .customStatus-1bh2V9 {
    width: 95%;
}

/*Profile window*/

.root-SR8cQa { /*Main modal*/
    border-radius: var(--general-radius);
    background-color: transparent;
    box-shadow: 0px 0px 5px 2px rgba(var(--main-accent), 0.85);
}
.root-SR8cQa::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background: var(--background-image);
    background-size: cover;
    border-radius: var(--general-radius);
    filter: brightness(0.1);
    z-index: -1;
}
.topSectionNormal-2-vo2m,
.topSectionPlaying-1J5E4n,
.headerFill-adLl4x,
.body-3ND3kc { /*Modal subcontainers*/
    background-color: transparent;
}
.tabBarContainer-1s1u-z,
.userInfoSection-2acyCx+.userInfoSection-2acyCx { /*Divider*/
    border-top: unset;
}
.connectedAccount-36nQx7 { /*Connected accounts profile*/
    border-color: transparent;
}
.tabBarItem-1b8RUP { /*Profile mutual tabs*/
    border: unset!important;
}
.tabBarItem-1b8RUP::before { /*Profile mutual tabs underline*/
    content: '';
    position: absolute;
    bottom: 10%;
    left: 0;
    height: 1px;
    width: 100%;
    border-radius: var(--general-radius);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    animation: unhoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.tabBarItem-1b8RUP:hover::before { /*Profile mutual tabs hovered underline*/
    animation: hoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.tabBarItem-1b8RUP[aria-selected="true"]::before { /*Profile mutual tabs selected underline*/
    animation: selectedItem 0.25s ease;
    animation-fill-mode: forwards;
}
.root-SR8cQa .listRow-hutiT_:hover { /*Hovered mutual server*/
    background-color: rgba(var(--main-color), 0.1);
    border-radius: var(--general-radius);
}
.connectedAccountOpenIcon-2cNbq5 { /*Connected account website*/
    color: rgb(var(--main-accent), 0.35);
    transition: color 0.25s ease;
}
.connectedAccountOpenIcon-2cNbq5:hover { /*Connected account website*/
    color: rgb(var(--main-accent), 1);
}
.topSectionSpotify-1lI0-P { /*Spotify playing*/
    background-color: transparent;
}

/*Stream modal*/

.tile-2w4k5N:hover .sourceThumbnail-27dolk { /*Hovering screen/app to share*/
    box-shadow: inset 0 0 0 2px rgb(var(--main-accent), 0.65);
}
.sourceThumbnail-27dolk.selected-1nOkyc { /*Selected screen/app to share*/
    box-shadow: inset 0 0 0 2px rgb(var(--main-accent), 0.95);
}
.container-OI6I9q .selected-P8xTeN { /*App/Screen selected tab*/
    border-color: transparent;
}
.container-OI6I9q .segmentControlOption-1vCKaY.item-1TLUig:first-of-type:before { /*Profile mutual tabs underline 1*/
    content: '';
    position: absolute;
    bottom: 10%;
    left: 3%;
    height: 1px;
    width: 20%;
    border-radius: var(--general-radius);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    animation: unhoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.container-OI6I9q .segmentControlOption-1vCKaY.item-1TLUig:last-of-type:before { /*Profile mutual tabs underline 2*/
    content: '';
    position: absolute;
    bottom: 10%;
    left: 26.2%;
    height: 1px;
    width: 14%;
    border-radius: var(--general-radius);
    background: rgb(var(--main-accent));
    box-shadow: 0px 0px 3px 1px rgb(var(--main-accent));
    animation: unhoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.container-OI6I9q .segmentControlOption-1vCKaY.item-1TLUig:not(.selected-P8xTeN):hover::before { /*Profile mutual tabs hovered underline*/
    animation: hoveredItem 0.25s ease;
    animation-fill-mode: forwards;
}
.container-OI6I9q .segmentControlOption-1vCKaY.item-1TLUig.selected-P8xTeN::before { /*Profile mutual tabs selected underline*/
    animation: selectedItem 0.25s ease;
    animation-fill-mode: forwards;
}
.modalContent-BM7Qeh .card-2Mz_4z { /*Streamming settings 1*/
    border-radius: var(--general-radius);
    border-color: transparent;
    background-color: rgba(var(--main-color), .25);
}
.settingsGroup-2NaPKC .formItemTitle-155OC0 { /*Quality titles*/
    text-align: center;
}
.modalContent-BM7Qeh:last-child .item-3T2z1R { /*Quality settings*/
    border-color: transparent;
    background-color: transparent;
}
.modalContent-BM7Qeh:last-child .selectorButton-EEUWed:not(.selectorButtonPremiumRequired-mKMbIu):hover .selectorText-2I7fQU:not(.selectorTextSelected-1ymya_) { /*Hovered quality*/
    color: rgba(var(--main-accent), .35);
    transition: color 0.25s ease;
}
.modalContent-BM7Qeh:last-child .item-3T2z1R .selectorTextSelected-1ymya_ { /*Selected quality*/
    color: rgb(var(--main-accent), 1);
    transition: color 0.25s ease;
}
.item-1tOPte[aria-checked="true"].colorDefault-2K3EoJ .radioSelection-1HmrQS { /*PiP change quality circle*/
    animation: selectedCircle 0.25s ease;
    animation-fill-mode: forwards;
}
.tile-2naSqK { /*Invite people background*/
    background-color: transparent;
}
.participantsButton-KYW-IW { /*Stream participants buttons*/
    background-color: transparent;
}
.participantsButton-KYW-IW:hover { /*Stream participants buttons hover*/
    background-color: transparent;
    color: rgb(var(--main-accent), 1);
}
.background-ujHpbY { /*Stream participants background*/
    background-color: transparent!important;
}

/*Server configuration*/

.item-1tOPte.colorBrand-ROmMP1 { /*Invite people button*/
    color: var(--interactive-normal);
}
.item-1tOPte:hover.colorBrand-ROmMP1 { /*Invite people button hover*/
    color: var(--interactive-active);
}
.scroller-305q3I { /*Roles container*/
    background-color: transparent;
}
.descriptionBox-1EKQKL { /*Description modal*/
    background-color: transparent;
}
.auditLog-3jNbM6,
.card-o7rAq-,
.card-1o0mns,
.copyInput-2rOSt7 { /*Containers*/
    border-radius: var(--general-radius);
    border: 1px solid;
    border-color: rgba(var(--main-color), 0.35)!important;
    background-color: transparent!important;
    transition: border-color 0.25s ease;
}
.auditLog-3jNbM6:hover,
.card-o7rAq-:hover,
.card-1o0mns:hover,
.copyInput-2rOSt7:hover { /*Containers hovered*/
    border-color: rgba(var(--main-accent), 0.85)!important;
}
.header-GwIGlr { /*Audit log subcointainer*/
    background-color: transparent!important;
}
.featureCard-1RR4Tl,
.featureIcon-3p1TC_ { /*Community features*/
    background-color: transparent;
}
.member-1q7VfX { /*Server member divider*/
    box-shadow: unset;
}
.card-FDVird:before { /*Hovered member*/
    background-color: rgb(var(--main-color))!important;
    border-color: transparent!important;
    filter: brightness(0.55);
}
.revokeInvite-28N8uj { /*Remove invite button*/
    background-color: transparent!important;
    box-shadow: unset!important;
}
.cardPrimaryEditable-3KtE4g { /*Widget image*/
    background-color: transparent;
}
.upsellContainer-L9xv7w,
.upsellFooter-ZYsio_ { /*Community overview header*/
    background-color: transparent;
}
.backgroundAccent-349kuI,
.developerPortalCtaWrapper-2XNafh { /*Server insight*/
    background-color: transparent;
}
.checklistContainer-mFJZEJ,
.checklistHeader-1KWcEY,
.separator-2V2oIO,
.separator-Hx_3SF { /*Partner program*/
    background-color: transparent;
}
.container-2w0lh0,
.header-2Y0-A-,
.separator-1COOpU { /*Discovery*/
    background-color: transparent;
}
.exampleContainer-3ekFIr,
.exampleModal-2oh58d,
.guildSidebar-339BqP,
.content-BMIBeK,
.formFieldWrapper-malor5,
.footer-1JuRYY,
.exampleContainer-25sB-A,
.exampleModal-2X2Vf8,
.optionContainer-1FtykV { /*Examples*/
    background-color: transparent!important;
}
.exampleContainer-3ekFIr,
.exampleContainer-25sB-A { /*Examples 2*/
    background-image: url('');
}
.fakeButton-kGEmb3 { /*fake submit button*/
    background-color: rgba(var(--main-accent), 0.4);
}
.exampleModal-2oh58d::before { /*Modal bakground*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgba(var(--main-color), 1);
    filter: brightness(0.25);
    z-index: -1;
}
.exampleTextSingleLine-1kvErc { /*example text color*/
    background-color: rgba(var(--main-color), 1)!important;
}
.titleContainer-2CXtJo { /*Admin role modal*/
    background-color: transparent;
}
.header-2mZ9Ov { /*Role sticky header*/
    background-color: transparent;
    border-radius: var(--general-radius);
}
.header-2mZ9Ov::before { /*Role sticky header background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), 1);
    filter: brightness(0.15);
    z-index: -1;
}
.container-cMG81i { /*Role sticky header searchbar*/
    background-color: rgba(var(--main-color), 0.3);
}
.tabBar-11f3uI {
    border-color: transparent;
}
.top-28JiJ- .brand-1Zl8en.item-PXvHYJ:active, .top-28JiJ- .brand-1Zl8en.selected-3s45Ha.item-PXvHYJ { /*Role sticky header tab*/
    color: rgba(var(--main-accent), 0.4);
    border-bottom-color: rgba(var(--main-accent), 0.4);
}
.container-2VW0UT { /*Unsaved changes*/
    background-color: rgba(var(--main-color), 0.25)!important;
    backdrop-filter: blur(5px);
}
.settingCard-3w2mVL,
.settingCard-3w2mVL.active-1ytUzX { /*Permissions main panel*/
    background: transparent;
}
.settingCard-3w2mVL { /*Permissions main panel*/
    border: 1px solid rgb(var(--main-accent), 1);
    border-radius: var(--general-radius);
}
.cardFolder-28dwxo { /*Permissions body*/
    background: transparent;
}
.group-1WdBVp { /*Permissions buttons*/ 
    border-color: transparent;
}
.item-1yAxl1 { /*Permissions buttons 2*/ 
    background-color: transparent;
}
.passthrough-1c2ewQ.selected-2YhbGh { /*Permissions buttons 3*/ 
    background-color: rgba(var(--main-color), .5);
}
.container-_phMUq { /*Role panel default permissions container*/
    background-color: transparent;
}
.container-_phMUq:hover,
.roleRow-30TwGe:hover:not(.roleRowDisableHover-1HiqqT) { /*Role panel default permissions container*/
    background-color: rgba(var(--main-color), .25);
}
.roleRow-30TwGe:hover:not(.roleRowDisableHover-1HiqqT) .circleButton-3RB01i,
.icon-3_8HGa { /*Role panel icons background*/
    background-color: transparent;
}

/*User card roles*/

.role-2irmRk { /*Role in user card*/
    position: relative;
    display: grid;
    border-radius: var(--general-radius);
    border: 0px;
    margin-right: 8px;
    margin-bottom: 8px;
}
.role-2irmRk > .roleCircle-3xAZ1j { /*Removes circle in role tag*/
    width: 0px;
    height: 0px;
}
.role-2irmRk > .roleCircle-3xAZ1j::after { /*Creates the background behind the role tag*/
    content: '';
    border-radius: var(--general-radius);
    position: absolute;
    left: 0px;
    top: 0px;
    bottom: 0px;
    right: 0px;
    background: inherit;
    filter: brightness(0.7)
}
.roleName-32vpEy { /*Tag text settings*/
    font-size: 105%;
    margin-left: 5px;
    margin-bottom: 1px;
    color: white!important;
    z-index: 3;
}

/*Misc*/

.attachButtonPlay-3iJ0mf { /*Attach Spotify group listen button*/
    color: rgb(var(--main-accent));
}
.ring-13rgEW { /*Focussed element when pressing tab*/
    box-shadow: unset;
}
.bd-toast { /*BD unloaded theme*/
    background: rgb(var(--main-color));
    border-radius: var(--general-radius);
}
.bd-toast.toast-success { /*BD applied theme*/
    background-color: rgba(var(--main-accent), 0.4);
    border-radius: var(--general-radius);
}
.checkboxWrapper-SkhIWG .checkbox-1ix_J3 { /*Checkmark box*/
    border-color: rgba(var(--main-color), 0.8)!important;
    background-color: transparent!important;
    transition: border-color 0.25s ease;
}
.checkboxWrapper-SkhIWG .checkbox-1ix_J3[style*="background-color: rgb(114, 137, 218);"],
.checkboxWrapper-SkhIWG .checkbox-1ix_J3.checked-3_4uQ9 { /*Checkmark checked color*/
    border-color: rgba(var(--main-accent), 1.2)!important;
    transition: border-color 0.25s ease;
}
.checkboxWrapper-SkhIWG .checkbox-1ix_J3[style*="background-color: rgb(114, 137, 218);"] svg path,
.checkboxWrapper-SkhIWG .checkbox-1ix_J3.checked-3_4uQ9 svg path { /*Checkmark check color*/
    fill: rgba(var(--main-accent), 1.2)!important;
    transition: 0.25s ease;
}
.checkboxWrapper-SkhIWG:hover .checkbox-1ix_J3:not([style*="background-color: rgb(114, 137, 218);"]):not(.checked-3_4uQ9){ /*Checkmark box hovered color*/
    border-color: rgba(var(--main-accent), 0.35)!important;
    transition: border-color 0.25s ease;
}
.colorDefault-2K3EoJ .checkbox-3s5GYZ { /*Hide muted channels checked checkmark box*/
    color: rgba(var(--main-accent), 0.65);
}
.colorDefault-2K3EoJ.focused-3afm-j .checkbox-3s5GYZ { /*Hide muted channels checked checkmark box hovered*/
    color: rgba(var(--main-accent), 0.35);
}
.colorDefault-2K3EoJ.focused-3afm-j .check-1JyqgN { /*Hide muted channels checked checkmark box hovered*/
    color: white;
}
.notice-2X5hT5 { /*Notice message*/
    background-color: rgba(var(--main-color), 0.35);
}
.keyboardShortcutsModal-3piNz7 { /*Main modal*/
    background-color: transparent!important;
    border-radius: var(--general-radius);
}
.keyboardShortcutsModal-3piNz7::before { /*Main modal background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background-color: rgb(var(--main-color));
    border-radius: var(--general-radius);
    filter: brightness(0.25);
    z-index: -1;
}
.keybindShortcut-1BD6Z1 span { /*Keybind button*/
    border-radius: var(--general-radius);
    background-color: rgb(var(--main-accent), 0.55)!important;
}
.dim-1l4L4y span { /*Keybind button*/
    background-color: rgb(var(--main-accent), 0.55)!important;
}
.dim-1l4L4y span:active { /*Keybind button pressed*/
    color: white!important;
}
.mediaBarGrabber-1FqnbN,
.mediaBarProgress-1xaPtl,
.mediaBarProgress-1xaPtl:after,
.mediaBarProgress-1xaPtl:before { /*Stream volume bar*/
    background-color: rgba(var(--main-accent), 0.85)!important;
}
.highlight { /*Highlight*/
    background-color: rgb(var(--main-accent), 0.1);
}
.required-7sPBq3 { /*Required input*/
    color: rgb(var(--main-accent), 1);
}

/*Minimal Mode*/
.bd-minimal .base-3dtUhz { /*Main modal*/
    left: 0;
}

/*Plugins compatibility*/

/*DevilBro's Server Folders*/
.lowerLeftBadge-zr4T_9 .numberBadge-2s8kKX,
.upperLeftBadge-e35IpL .numberBadge-2s8kKX { /*DevilBro's Server Folders badges*/
    background-color: transparent!important;
}
.lowerLeftBadge-zr4T_9 .numberBadge-2s8kKX::before,
.upperLeftBadge-e35IpL .numberBadge-2s8kKX::before { /*DevilBro's Server Folders badges background*/
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    border-radius: var(--avatar-radius);
    background-color: rgb(var(--main-accent));
    filter: brightness(0.5);
    z-index: -1;
}
.baseShapeRound-1Mm1YW { /*Badges radius*/
    border-radius: var(--general-radius);
}

/*Member Count*/
#MemberCount { /*Styling*/
    margin-left: 8px!important;
    background: transparent!important;
}

/*GooseMod compatibility*/

.children-rWhLdy div[style*="background-color: var(--background-secondary);"] { /*Main elements background*/
    background-color: transparent!important;
}
.children-rWhLdy div[style*="display: grid;"] div { /*Main elements addons*/
    z-index: 2!important;
}
.children-rWhLdy div[style*="display: grid;"] div[style*="width: calc(100% - 32px);"] { /*Main elements addons*/
    width: auto!important;
}
.children-rWhLdy div[style*="display: grid;"] > div::before { /*Main elements addons background*/
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    border-radius: var(--general-radius);
    background-color: rgba(var(--main-color), .25)!important;
    z-index: -1;
}
.children-rWhLdy div[style*="display: grid;"] div .control-2BBjec { /*Main elements addons background*/
    left: 245px!important;
}
.children-rWhLdy div[style*="width: 100%;"] .titleDefault-a8-ZSr { /*Module count/tags*/
    background-color: transparent!important;
    pointer-events: none;
    border-radius: unset!important;
    border-bottom: 1px solid rgba(var(--main-accent), 1);
}
.sidebarRegion-VFTUkN { /*Removes weird left movement*/
    max-width: unset!important;
}
