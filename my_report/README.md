# Lesson: Interaction Design

### First and Last Name: Maria Siafali
### University Registration Number: dpsd19117
### GitHub Personal Profile: https://github.com/MariaSiafali117
### Augmented Reality Personal Repository: https://mariasiafali117.github.io/Augmented-Reality/marker_based/index.html

# Introduction

# Summary


# 1st Deliverable
Για την εργασία αυτή αξιοποίησα τα προτεινόμενα λινκ για να βρω τις κατάλληλες εντολές για την σφαίρα, τον κύλινδρο, το κουτί, το χιόνι και τις φωνητικές εντολές που σταματούν την ροή του χιονιού και την επαναξεκινούν. Κατα την εκτέλεση του προγράματος αντιμετώπισα κάποια προβλήματα. Συγκεκριμένα το χιόνι θα προτειμούσα να είναι λίγο πιο πυκνό αλλά δεν μπόρεσα να το κάνω, παρ'όλα αυτά δουλεύει κανονικά. Επίσης ενώ δεν υπάρχει κάποιο πρόβλημα με τις φωνητικές εντολές στον κώδικα, δεν σταματάει στην εντολή stop και αντίστοιχα δεν ξεκίναει με την εντολή start. Προκειμένου να κάνω την εργασία, κατέβασα την python στον υπολογιστή μου, την ενεργοποίησα μέσω της εφαρμογής PowerShell, βρήκα τον φάκελο με το αρχείο index του marker based το οπόιο το κατέβασα μέσω της εφαρμογήσ github dekstop στον υπολογιστή μου. Έπειτα άνοιξα τον αρχείο με τον κώδικα μέσω της εφαρμογή visual studio code και έκανα τις απαραίτητες αλλαγές. Για να κάνω τις αλλαγές που έπρεπε πειραματήστηκα προκειμένου να βρω τις κατάλληες τιμές που ήθελα. Αφού έτρεξα τον κώδικα μέσω της python και είδα ότι δουλεύει, ανέβασα το αρχείο στο προσωπικό μου λινκ για την εργασία Augment-Reality marker based. Ο κώδικας που έγραψα είναι ο εξής:


<!DOCTYPE html>
<html>
    <script src="https://aframe.io/releases/1.0.0/aframe.min.js"></script>
    <!-- we import arjs version without NFT but with marker + location based support -->
    <!--<script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>-->
    <script src="build/aframe-ar.js"></script>
    
    <!-- particles system component -->
    <script src="https://unpkg.com/aframe-particle-system-component@1.0.x/dist/aframe-particle-system-component.min.js"></script>
    
    <!-- speech command component -->
    <script src="//cdnjs.cloudflare.com/ajax/libs/annyang/2.5.0/annyang.min.js"></script>
    <script src="build/aframe-speech-command-component.js"></script> 
    

    <body style="margin : 0px; overflow: hidden;">
        <a-scene vr-mode-ui="enabled: false;"
                 renderer="logarithmicDepthBuffer: true;"
                 embedded
                 arjs="trackingMethod: best; sourceType: webcam;debugUIEnabled: false;">

            <a-entity id="annyang" annyang-speech-recognition></a-entity>

            <a-entity id="switch"
                      speech-command__start ="command: start; type: attribute; attribute: visible; value: true;"
                      speech-command__stop ="command: stop; type: attribute; attribute: visible; value: false;">     
            </a-entity>

            <a-entity position="0 2.25 -15"  particle-system="preset: snow">  </a-entity>

            <a-marker preset="hiro">

                <a-box position="0 0 0" rotation="0 45 0" color="#53225D"></a-box>
                <a-sphere position="0.6 0.5 0.7" radius="0.35" color="#681E40"></a-sphere>
                <a-cylinder position="1.25 0 1.3" radius="0.5" height="1" color="#1E5D5D"></a-cylinder>

            </a-marker>
            <a-entity camera></a-entity>
        </a-scene>
       
    </body>
</html>

# 2nd Deliverable


# 3rd Deliverable 


# Conclusions


# Sources
