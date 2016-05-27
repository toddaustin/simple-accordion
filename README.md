# A simple jquery accordion


 
var allAccordion = $('.accordion > div').hide();

$('.accordion > p').click(function() {
  if ( $(this).next().is(':visible') ) {
    allAccordion.hide('fast');
    return false;
  } else {
    //close accordion
    allAccordion.hide('fast');
}

//open accordion
$(this).next().slideDown("slow");
  return false;
});
