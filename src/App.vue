<template>
  <div id="app" class="mt-172 zeromargin">
    <chat-card></chat-card>
  </div>
</template>

<script>
import ChatCard from "./components/FIlterCard";
export default {
  name: "App",
  components: {
    "chat-card": ChatCard
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.mt-172 {
  margin-top: 172px;
}

@media screen and (max-width: 600px) {
  .mt-172 {
    margin-top: 44px;
  }
}

.material-icons {
  font-family: "Material Icons";
  font-weight: normal;
  font-style: normal;
  font-size: 24px;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  display: inline-block;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-feature-settings: "liga";
  -webkit-font-smoothing: antialiased;
}
.application a {
  cursor: pointer;
}
.theme--light.v-icon {
  color: rgba(0, 0, 0, 0.54);
}
.v-icon {
  -webkit-box-align: center;
  align-items: center;
  display: -webkit-inline-box;
  display: inline-flex;
  font-feature-settings: "liga";
  font-size: 24px;
  -webkit-box-pack: center;
  justify-content: center;
  line-height: 1;
  -webkit-transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
  vertical-align: text-bottom;
}
.v-input--selection-controls {
  margin-top: 16px;
  padding-top: 4px;
}
.v-input--selection-controls .v-input__control {
  -webkit-box-flex: 0;
  flex-grow: 0;
  width: auto;
}
.v-input--selection-controls:not(.v-input--hide-details) .v-input__slot {
  margin-bottom: 12px;
}
.v-input--selection-controls__input {
  color: inherit;
  display: -webkit-inline-box;
  display: inline-flex;
  -webkit-box-flex: 0;
  flex: 0 0 auto;
  height: 24px;
  position: relative;
  margin-right: 8px;
  -webkit-transition: 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  -webkit-transition-property: color, -webkit-transform;
  transition-property: color, -webkit-transform;
  transition-property: color, transform;
  transition-property: color, transform, -webkit-transform;
  width: 24px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.v-input--selection-controls__input input {
  position: absolute;
  opacity: 0;
  width: 100%;
  height: 100%;
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.v-input--selection-controls__ripple {
  border-radius: 50%;
  cursor: pointer;
  height: 34px;
  position: absolute;
  -webkit-transition: inherit;
  transition: inherit;
  width: 34px;
  left: -12px;
  top: calc(50% - 24px);
  margin: 7px;
}
.v-input--selection-controls__ripple:before {
  border-radius: inherit;
  bottom: 0;
  content: "";
  position: absolute;
  opacity: 0.2;
  left: 0;
  right: 0;
  top: 0;
  -webkit-transform-origin: center center;
  transform-origin: center center;
  -webkit-transform: scale(0.2);
  transform: scale(0.2);
  -webkit-transition: inherit;
  transition: inherit;
}
.theme--light.v-input:not(.v-input--is-disabled) input {
  color: rgba(0, 0, 0, 0.87);
}
.theme--light.v-input input::-webkit-input-placeholder {
  color: rgba(0, 0, 0, 0.38);
}
.theme--light.v-input input::-moz-placeholder {
  color: rgba(0, 0, 0, 0.38);
}
.theme--light.v-input input:-ms-input-placeholder {
  color: rgba(0, 0, 0, 0.38);
}
.theme--light.v-input input::-ms-input-placeholder {
  color: rgba(0, 0, 0, 0.38);
}
.theme--light.v-input input::placeholder {
  color: rgba(0, 0, 0, 0.38);
}
.v-input {
  -webkit-box-align: start;
  align-items: flex-start;
  display: -webkit-box;
  display: flex;
  -webkit-box-flex: 1;
  flex: 1 1 auto;
  font-size: 16px;
  text-align: left;
}
.v-input input {
  max-height: 32px;
}
.v-input input:invalid {
  box-shadow: none;
}
.v-input input:focus,
.v-input input:active {
  outline: none;
}
.v-input__control {
  display: -webkit-box;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  flex-direction: column;
  height: auto;
  -webkit-box-flex: 1;
  flex-grow: 1;
  flex-wrap: wrap;
  width: 100%;
}
.v-input__slot {
  -webkit-box-align: center;
  align-items: center;
  color: inherit;
  display: -webkit-box;
  display: flex;
  margin-bottom: 8px;
  min-height: inherit;
  position: relative;
  -webkit-transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
  width: 100%;
}
.theme--light.v-messages {
  color: rgba(0, 0, 0, 0.54);
}
.v-messages {
  -webkit-box-flex: 1;
  flex: 1 1 auto;
  font-size: 12px;
  min-height: 12px;
  min-width: 1px;
  position: relative;
}

.container {
  -webkit-box-flex: 1;
  flex: 1 1 100%;
  margin: auto;
  padding: 24px;
  width: 100%;
}
@media only screen and (min-width: 960px) {
  .container {
    max-width: 900px;
  }
}
@media only screen and (min-width: 1264px) {
  .container {
    max-width: 1185px;
  }
}
@media only screen and (min-width: 1904px) {
  .container {
    max-width: 1785px;
  }
}
@media only screen and (max-width: 959px) {
  .container {
    padding: 16px;
  }
}

*,
::before,
::after {
  box-sizing: inherit;
}
::before,
::after {
  text-decoration: inherit;
  vertical-align: inherit;
}
* {
  background-repeat: no-repeat;
  padding: 0;
  margin: 0;
}
hr {
  overflow: visible;
}
a {
  background-color: transparent;
  -webkit-text-decoration-skip: objects;
}
a:active,
a:hover {
  outline-width: 0;
}
b {
  font-weight: bolder;
}
input {
  border-radius: 0;
}
button,
[role="button"] {
  cursor: pointer;
}
textarea {
  overflow: auto;
  resize: vertical;
}
button,
input,
textarea {
  font: inherit;
}
button {
  overflow: visible;
}
button::-moz-focus-inner {
  border-style: 0;
  padding: 0;
}
button:-moz-focusring {
  outline: 0;
  border: 0;
}
button {
  -webkit-appearance: button;
}
button {
  text-transform: none;
}
button,
input,
textarea {
  background-color: transparent;
  border-style: none;
  color: inherit;
}
img {
  border-style: none;
}
svg:not(:root) {
  overflow: hidden;
}
::-moz-selection {
  background-color: #b3d4fc;
  color: #000;
  text-shadow: none;
}
::selection {
  background-color: #b3d4fc;
  color: #000;
  text-shadow: none;
}
::-ms-clear,
::-ms-reveal {
  display: none;
}
ul {
  padding-left: 24px;
}
p {
  margin-bottom: 16px;
}

.close {
  margin: 10px;
}

h5 {
  margin-bottom: 0;
}

a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
b {
  font-weight: 700;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
hr {
  box-sizing: content-box;
  height: 0;
}
button,
input,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
@media print {
  *,
  :after,
  :before {
    color: #000 !important;
    text-shadow: none !important;
    background: 0 0 !important;
    box-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  a[href^="#"]:after {
    content: "";
  }
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p {
    orphans: 3;
    widows: 3;
  }
}
* {
  box-sizing: border-box;
}
:after,
:before {
  box-sizing: border-box;
}
button,
input,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:focus,
a:hover {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
img {
  vertical-align: middle;
}
hr {
  margin-top: 20px;
  margin-bottom: 20px;
  border: 0;
  border-top: 1px solid #eee;
}
[role="button"] {
  cursor: pointer;
}
h4,
h5 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h4,
h5 {
  margin-top: 10px;
  margin-bottom: 10px;
}
h4 {
  font-size: 18px;
}
h5 {
  font-size: 14px;
}
p {
  margin: 0 0 10px;
}
.text-left {
  text-align: left;
}
ul {
  margin-top: 0;
  margin-bottom: 10px;
}
ul ul {
  margin-bottom: 0;
}
.container {
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
}
@media (min-width: 768px) {
  .container {
    width: 750px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 970px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1170px;
  }
}
.row {
  margin-right: -15px;
  margin-left: -15px;
}
.col-sm-12,
.col-sm-4,
.col-sm-6,
.col-sm-8 {
  position: relative;
  min-height: 1px;
  padding-right: 15px;
  padding-left: 15px;
}
@media (min-width: 768px) {
  .col-sm-12,
  .col-sm-4,
  .col-sm-6,
  .col-sm-8 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: 700;
}
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px\9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="checkbox"]:focus,
input[type="file"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.form-control {
  display: block;
  width: 100%;
  height: 34px;
  padding: 6px 12px;
  font-size: 14px;
  line-height: 1.42857143;
  color: #555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out 0.15s,
    box-shadow ease-in-out 0.15s;
  -webkit-transition: border-color ease-in-out 0.15s,
    -webkit-box-shadow ease-in-out 0.15s;
  transition: border-color ease-in-out 0.15s, box-shadow ease-in-out 0.15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075),
    0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  background-color: transparent;
  border: 0;
}
textarea.form-control {
  height: auto;
}
.form-group {
  margin-bottom: 15px;
}
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.checkbox input[type="checkbox"] {
  position: absolute;
  margin-top: 4px\9;
  margin-left: -20px;
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: 400;
  text-align: center;
  white-space: nowrap;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  padding: 6px 12px;
  font-size: 14px;
  line-height: 1.42857143;
  border-radius: 4px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:active:focus,
.btn:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:focus,
.btn:hover {
  color: #333;
  text-decoration: none;
}
.btn:active {
  background-image: none;
  outline: 0;
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active {
  color: #fff;
  background-color: #449d44;
  background-image: none;
  border-color: #398439;
}
.btn-success:active:focus,
.btn-success:active:hover {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active {
  color: #fff;
  background-color: #c9302c;
  background-image: none;
  border-color: #ac2925;
}
.btn-danger:active:focus,
.btn-danger:active:hover {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-sm {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 3px;
}
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  font-size: 14px;
  text-align: left;
  list-style: none;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 4px;
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: 400;
  line-height: 1.42857143;
  color: #333;
  white-space: nowrap;
}
.dropdown-menu > li > a:focus,
.dropdown-menu > li > a:hover {
  color: #262626;
  text-decoration: none;
  background-color: #f5f5f5;
}
.dropdown-menu-right {
  right: 0;
  left: auto;
}
.btn-group {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group .dropdown-toggle:active {
  outline: 0;
}
.chat-template .chat-section .chat-scroller .received-msg .text-wrapper .time,
.chat-template .chat-section .chat-scroller .sent-msg .text-wrapper .time {
  -webkit-box-flex: 1;
  flex-grow: 1;
  text-align: right;
  color: grey;
  font-size: 12px;
  padding: 5px;
}
.chat-template .chat-section .chat-scroller .received-msg .profile-image {
  width: 40px;
  height: 40px;
  margin-top: 7px;
  border-radius: 50%;
  float: left;
  position: relative;
  background-position: center;
  background-size: cover;
}
.chat-template .chat-section .chat-scroller .received-msg .text-wrapper .image,
.chat-template .chat-section .chat-scroller .sent-msg .text-wrapper .image {
  display: -webkit-box;
  display: flex;
  flex-wrap: wrap;
  -webkit-box-pack: end;
  justify-content: flex-end;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  flex-flow: column;
  position: relative;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .text-wrapper
  .image
  .overlay,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .image
  .overlay {
  display: none;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .text-wrapper
  .image:hover
  .overlay,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .image:hover
  .overlay {
  display: block;
  background-image: -webkit-gradient(
    linear,
    left top,
    right bottom,
    from(rgba(0, 0, 0, 0.87)),
    to(rgba(0, 0, 0, 0.54))
  );
  background-image: linear-gradient(
    to bottom right,
    rgba(0, 0, 0, 0.87),
    rgba(0, 0, 0, 0.54)
  );
  position: absolute;
  width: 100%;
  height: 200px;
  top: 0;
  left: 0;
  opacity: 0.7;
  margin: 0;
  z-index: 10;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .text-wrapper
  .image
  img,
.chat-template .chat-section .chat-scroller .sent-msg .text-wrapper .image img {
  width: auto;
  height: 200px;
  border-radius: 0;
}
.chat-template .chat-section .chat-scroller .received-msg .file-types {
  display: -webkit-box;
  display: flex;
  -webkit-box-align: center;
  align-items: center;
}
.chat-template .chat-section .chat-scroller .received-msg .file-types .svg {
  height: 45px;
}
.chat-template .chat-section .chat-scroller .received-msg .file-types .svg svg {
  height: 45px;
  width: auto;
  padding: 5px;
  margin: 0 5px 0 0;
  border: 1px solid #eee;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .file-types
  .svg
  i.fas {
  font-size: 19px;
  position: absolute;
  margin-left: -16px;
  bottom: 10px;
  color: #009f9a;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .file-types
  .text-type {
  padding-left: 5px;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .file-types
  .text-type
  p {
  margin: 0;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .file-types
  .text-type
  span {
  font-size: 11px;
  color: grey;
}
.chat-template .chat-section .chat-scroller .received-msg .reply,
.chat-template .chat-section .chat-scroller .sent-msg .text-wrapper .reply {
  width: -webkit-max-content;
  width: -moz-max-content;
  width: max-content;
  max-width: 100%;
}
.chat-template .chat-section .chat-scroller .received-msg .reply .text svg,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text
  svg {
  fill: #1e1d21;
  margin: 9px;
}
.chat-template .chat-section .chat-scroller .received-msg .reply .text .inner,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text
  .inner {
  background: white;
  padding: 10px;
  border-radius: 4px;
  border-left: 5px solid #009f9a;
  display: flow-root;
}
.chat-template .chat-section .chat-scroller .received-msg .reply .text .inner p,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text
  .inner
  p {
  color: #009f9a;
  font-weight: bold;
  margin-bottom: 2px;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .reply
  .text
  .inner
  img {
  width: 80px;
  height: auto;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .reply
  .text:nth-child(1),
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text:nth-child(1) {
  border-radius: 10px 10px 0 0;
  padding: 10px 10px 2px;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .reply
  .text:nth-child(2),
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text:nth-child(2) {
  border-radius: 0 0 0 10px;
  padding: 5px 10px 10px 10px;
}
.chat-template .chat-section .chat-scroller .received-msg .check-flex,
.chat-template .chat-section .chat-scroller .sent-msg .check-flex {
  display: -webkit-box;
  display: flex;
  -webkit-box-align: center;
  align-items: center;
  width: 100%;
}
.chat-template .chat-section .chat-scroller .received-msg .check-flex .checkbox,
.chat-template .chat-section .chat-scroller .sent-msg .check-flex .checkbox {
  display: none;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .check-flex
  .checkbox
  .v-input--selection-controls,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .check-flex
  .checkbox
  .v-input--selection-controls {
  margin: 0;
  padding: 0;
  height: 24px;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .check-flex
  .checkbox
  .v-input--selection-controls
  .v-input__slot,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .check-flex
  .checkbox
  .v-input--selection-controls
  .v-input__slot {
  margin: 0;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .check-flex
  .checkbox
  .v-input--selection-controls
  .v-input__slot
  .v-input--selection-controls__input,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .check-flex
  .checkbox
  .v-input--selection-controls
  .v-input__slot
  .v-input--selection-controls__input {
  margin: 0;
}
.chat-template .chat-section .chat-scroller .received-msg .btn-group.dropdown,
.chat-template .chat-section .chat-scroller .sent-msg .btn-group.dropdown {
  display: none;
  z-index: 11;
}
.chat-template .chat-section .chat-scroller .received-msg .dropdown-menu-right,
.chat-template .chat-section .chat-scroller .sent-msg .dropdown-menu-right {
  right: 0;
  margin-top: -7px;
  padding: 0;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .dropdown-menu-right
  li,
.chat-template .chat-section .chat-scroller .sent-msg .dropdown-menu-right li {
  border: 0;
  padding: 5px 16px;
  border-bottom: 1px solid #eee;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .dropdown-menu-right
  li:last-child,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .dropdown-menu-right
  li:last-child {
  border: 0;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .text-wrapper
  .image:hover
  .btn-group.dropdown,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .image:hover
  .btn-group.dropdown,
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .reply
  .text:hover
  .btn-group.dropdown,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text:hover
  .btn-group.dropdown,
.chat-template
  .chat-section
  .chat-scroller
  .received-msg:hover
  .btn-group.dropdown,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg:hover
  .btn-group.dropdown {
  position: absolute;
  right: 10px;
  display: block;
  top: 5px;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .text-wrapper
  .image:hover
  .btn-group.dropdown
  a,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .image:hover
  .btn-group.dropdown
  a,
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .reply
  .text:hover
  .btn-group.dropdown
  a,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text:hover
  .btn-group.dropdown
  a,
.chat-template
  .chat-section
  .chat-scroller
  .received-msg:hover
  .btn-group.dropdown
  a,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg:hover
  .btn-group.dropdown
  a {
  box-shadow: none;
}
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .text-wrapper
  .image:hover
  .btn-group.dropdown
  a
  svg,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .image:hover
  .btn-group.dropdown
  a
  svg,
.chat-template
  .chat-section
  .chat-scroller
  .received-msg
  .reply
  .text:hover
  .btn-group.dropdown
  a
  svg,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg
  .text-wrapper
  .reply
  .text:hover
  .btn-group.dropdown
  a
  svg,
.chat-template
  .chat-section
  .chat-scroller
  .received-msg:hover
  .btn-group.dropdown
  a
  svg,
.chat-template
  .chat-section
  .chat-scroller
  .sent-msg:hover
  .btn-group.dropdown
  a
  svg {
  width: 10px;
}
.chat-template .date-of-messages {
  text-align: center;
  position: relative;
  margin: 20px;
}
.chat-template .date-of-messages span {
  display: inline-block;
}
.chat-template .date-of-messages span:before,
.chat-template .date-of-messages span:after {
  border-top: 1px solid #eee;
  display: block;
  height: 1px;
  content: " ";
  width: 40%;
  position: absolute;
  left: 0;
  top: 0.8em;
}
.chat-template .date-of-messages span:after {
  right: 0;
  left: auto;
}
.chat-template .date-of-messages span.yesterday:before,
.chat-template .date-of-messages span.yesterday:after {
  width: 44%;
}
.chat-template .container.res {
  padding-top: 0;
  margin: 10px auto;
}
.chat-template .sidebar {
  display: flow-root;
  border-right: 1px solid #eee;
  min-height: 80vh;
}
.chat-template .sidebar .search {
  display: flow-root;
  border-bottom: 1px solid #eee;
  padding-bottom: 15px;
}
.chat-template .sidebar .tabs {
  border-bottom: 1px solid #eee;
  display: flow-root;
  margin-bottom: 15px;
  box-shadow: -1px 3px 3px #eeeeee73;
}
.chat-template .sidebar .tabs .icons {
  width: -webkit-max-content;
  width: -moz-max-content;
  width: max-content;
  float: left;
  width: 25%;
  position: relative;
  cursor: pointer;
}
.chat-template .sidebar .tabs .icons.active p {
  color: #009f9a;
}
.chat-template .sidebar .tabs .icons.active:after {
  content: "";
  position: absolute;
  right: 0%;
  border-bottom: 2px solid #009f9a;
  height: 100%;
  top: 3%;
  width: 100%;
}
.chat-template .sidebar .tabs .icons img {
  max-width: 25%;
  display: block;
  margin: auto;
}
.chat-template .sidebar .tabs .icons p {
  text-align: center;
}
.chat-template .sidebar .chat-scroller {
  height: 66vh;
  overflow: auto;
}
.chat-template .sidebar .chat-scroller::-webkit-scrollbar {
  display: none;
}
.chat-template .sidebar .chat-scroller ul.lister {
  list-style: none;
  display: flow-root;
  padding: 0;
  padding-bottom: 60px;
}
.chat-template .sidebar .chat-scroller .button-container {
  position: absolute;
  bottom: 0;
  width: 100%;
  background: white;
  padding: 15px;
  border-right: 1px solid #eee;
  border-top: 1px solid #eee;
  box-shadow: 0px -1px 3px #eee;
}
.chat-template .sidebar .chat-scroller .button-container .btn {
  width: 100%;
  margin: 0;
}
.chat-template .sidebar-template {
  position: absolute;
  top: 0;
  background: white;
  width: 42%;
  height: 80.2vh;
  border-left: 1px solid #eee;
  right: 0;
  z-index: 100;
  overflow: hidden;
  overflow-y: auto;
}
.chat-template .sidebar-template img.edit {
  width: 20px;
  right: 43px;
  position: absolute;
  top: 9px;
  opacity: 0.7;
}
.chat-template .sidebar-template::-webkit-scrollbar-track {
  display: none;
}
.chat-template .sidebar-template::-webkit-scrollbar {
  width: 3px;
  border-radius: 0;
}
.chat-template .sidebar-template::-webkit-scrollbar-thumb {
  background: #eee;
}
.chat-template .sidebar-template .member-list .lister li {
  padding: 10px 5px 15px;
}
.chat-template .sidebar-template .member-list .lister li p {
  text-align: left;
}
.chat-template .sidebar-template .member-list .lister li ul.dropdown-menu li {
  padding: 5px;
  border: 0;
  border-bottom: 1px solid #eee;
}
.chat-template
  .sidebar-template
  .member-list
  .lister
  li
  ul.dropdown-menu
  li:last-child {
  border: 0;
}
.chat-template .sidebar-template .member-list .lister li .profile-image {
  width: 50px;
  border-radius: 50%;
  height: 50px;
  background-position: center;
  background-size: cover;
}
.chat-template .sidebar-template .member-list .lister li .text-wrapper {
  width: calc(100% - 62px);
  padding-left: 8px;
  margin-top: -2px;
  display: flow-root;
}
.chat-template .sidebar-template .member-list .lister li .text-wrapper p,
.chat-template .sidebar-template .member-list .lister li .text-wrapper span {
  text-align: left;
}
.chat-template .sidebar-template .member-list .lister li .btn-group.dropdown {
  position: absolute;
  right: 10px;
  margin-top: -40px;
}
.chat-template .sidebar-template .member-list .lister li svg {
  width: 15px;
  display: none;
}
.chat-template .sidebar-template .member-list .lister li:hover svg {
  display: block;
}
.chat-template .sidebar-template .starred {
  margin-top: 15px;
}
.chat-template .sidebar-template .starred ul {
  list-style: none;
  padding: 0;
}
.chat-template .sidebar-template .starred ul li {
  padding: 15px;
  border-top: 1px solid #eee;
  cursor: pointer;
}
.chat-template .sidebar-template .starred ul li:last-child {
  border-bottom: 1px solid #eee;
}
.chat-template .sidebar-template .starred ul li svg {
  width: 20px;
  height: 20px;
  margin: -3px 10px;
}
.chat-template .sidebar-template h5 {
  width: -webkit-max-content;
  width: -moz-max-content;
  width: max-content;
  margin-left: -10px;
}
.chat-template .sidebar-template .nomar {
  margin: 0;
}
.chat-template .sidebar-template .close {
  width: 20px;
  position: absolute;
  right: 0px;
  z-index: 11;
}
.chat-template .sidebar-template .images .profile-image {
  width: 31%;
  border-radius: 0;
  height: 60px;
  float: left;
  cursor: pointer;
  flex-basis: 0 0 30%;
  max-width: 31%;
  -webkit-box-flex: 0;
  flex: 0 0 31%;
  margin: 1.1%;
}
.chat-template .sidebar-template .profile-image {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  background-position: center;
  margin: auto;
  margin-top: 2vh;
}
.chat-template .sidebar-template p {
  margin: 0;
  margin-top: 10px;
  text-align: center;
  color: #000;
}
.chat-template .sidebar-template span {
  width: 100%;
  text-align: center;
  color: grey;
  display: block;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}
.chat-template .chat-section .top-bar {
  border-bottom: 1px solid #eee;
  padding: 13px;
  display: flow-root;
  box-shadow: 0px 1px 3px #eee;
}
.chat-template .chat-section .top-bar .profile-section {
  width: -webkit-max-content;
  width: -moz-max-content;
  width: max-content;
  float: left;
  display: flow-root;
}
.chat-template .chat-section .top-bar .profile-section .profile-image {
  width: 40px;
  height: 40px;
  background-position: center;
  background-size: cover;
  border-radius: 50%;
  float: left;
}
.chat-template .chat-section .top-bar .profile-section .text-wrapper {
  padding-left: 10px;
  display: flow-root;
}
.chat-template .chat-section .top-bar .profile-section .text-wrapper p {
  margin: 0;
  color: #000;
}
.chat-template .chat-section .top-bar .profile-section .text-wrapper span {
  font-size: 13px;
}
.chat-template .chat-section .top-bar .profile-section .text-wrapper span a {
  color: grey;
}
.chat-template .chat-section .top-bar .menu-section {
  display: flow-root;
  width: -webkit-max-content;
  width: -moz-max-content;
  width: max-content;
  float: right;
}
.chat-template .chat-section .top-bar .menu-section ul.dropdown-menu {
  width: 245px;
  margin-right: 20px;
}
.chat-template .chat-section .top-bar .menu-section .form-control {
  display: none;
}
.chat-template .chat-section .top-bar .menu-section .form-control.menu {
  display: block;
  position: absolute;
  width: 31%;
  right: 22%;
}
.chat-template .chat-section .top-bar .menu-section img {
  height: 20px;
  cursor: pointer;
  margin: 10px 15px;
}
.chat-template .chat-section .chat-scroller {
  height: 66.2vh;
  padding: 15px;
  overflow: hidden;
  overflow-y: auto;
}
</style>
