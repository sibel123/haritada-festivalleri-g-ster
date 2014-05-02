haritada-festivalleri-g-ster
============================
//Setting the position of the Glastonbury map marker.
var markerPositionGlastonbury = new google.maps.LatLng(51.159803, -2.585585);
 
//Setting the icon to be used with the Glastonbury map marker.
var markerIconGlastonbury = {
 url: 'icons/icon_glas_uk.png',
 //The size image file.
 size: new google.maps.Size(225, 120),
 //The point on the image to measure the anchor from. 0, 0 is the top left.
 origin: new google.maps.Point(0, 0),
 //The x y coordinates of the anchor point on the marker. e.g. If your map marker was a drawing pin then the anchor would be the tip of the pin.
 anchor: new google.maps.Point(189, 116)
};
 
//Setting the shape to be used with the Glastonbury map marker.
var markerShapeGlastonbury = {
 coord: [12,4,216,22,212,74,157,70,184,111,125,67,6,56],
 type: 'poly'
};
 
//Creating the Glastonbury map marker.
markerGlastonbury = new google.maps.Marker({
 //uses the position set above.
 position: markerPositionGlastonbury,
 //adds the marker to the map.
 map: festivalMap,
 title: 'Glastonbury Festival',
 //assigns the icon image set above to the marker.
 icon: markerIconGlastonbury,
 //assigns the icon shape set above to the marker.
 shape: markerShapeGlastonbury,
 //sets the z-index of the map marker.
 zIndex:102
});
