# crop-zoom-pan

<div id="image-cropper">
  <div class="cropit-preview"></div>
  
  <input type="range" class="cropit-image-zoom-input" />
  
  <!-- The actual file input will be hidden -->
  <input type="file" class="cropit-image-input" />
  <!-- And clicking on this button will open up select file dialog -->
  <div class="select-image-btn">Select new image</div>
</div>
$('#image-cropper').cropit();

// When user clicks select image button,
// open select file dialog programmatically
$('.select-image-btn').click(function() {
  $('.cropit-image-input').click();
});

// Handle rotation
$('.rotate-cw-btn').click(function() {
  $('#image-cropper').cropit('rotateCW');
});
$('.rotate-ccw-btn').click(function() {
  $('#image-cropper').cropit('rotateCCW');
});
/* Hide file input */
input.cropit-image-input {
  visibility: hidden;
}

/*
 * See http://www.htmllion.com/html5-range-input-with-css.html
 * for styling range input
 */
 
