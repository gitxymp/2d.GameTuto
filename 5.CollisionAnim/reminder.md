ctx.fillStyle = "white";
ctx.fillRect(
e.x - canvasPosition.left - 25,
e.y - canvasPosition.top - 25,
50,
50
);

---

window.addEventListener("mousemove", function (e) {
createAnimation(e);
});

function createAnimation(e) {
let positionX = e.x - canvasPosition.left;
let positionY = e.y - canvasPosition.top;
explosions.push(new Explosion(positionX, positionY));
}
