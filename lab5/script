/* 
Name: Jaden Plummer
File: index.js
Date: 22 April 2026
Scripts for Assignment 5 - Web Accessibility
*/

// Show / Hide comments section

const showHideBtn = document.querySelector('.show-hide');
const commentWrapper = document.querySelector('.comment-wrapper');

commentWrapper.style.display = 'none';

showHideBtn.onclick = function () {
  if (showHideBtn.textContent === 'Show comments') {
    showHideBtn.textContent = 'Hide comments';
    commentWrapper.style.display = 'block';
  } else {
    showHideBtn.textContent = 'Show comments';
    commentWrapper.style.display = 'none';
  }
};

// Add new comment

const form = document.querySelector('.comment-form');
const nameField = document.querySelector('#name');
const commentField = document.querySelector('#comment');
const list = document.querySelector('.comment-container');

form.onsubmit = function (e) {
  e.preventDefault();

  const listItem = document.createElement('li');
  const namePara = document.createElement('p');
  const commentPara = document.createElement('p');

  namePara.textContent = nameField.value;
  commentPara.textContent = commentField.value;

  list.appendChild(listItem);
  listItem.appendChild(namePara);
  listItem.appendChild(commentPara);

  // clear inputs after submit
  nameField.value = '';
  commentField.value = '';
};
