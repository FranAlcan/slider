# slider
.slider-container {
	position: fixed;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	overflow: hidden;
	z-index: -1;
}

.slider-container img {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	opacity: 0;
	transition: opacity 2s ease-in-out;
}

.slider-container img:first-child {
	opacity: 1;
}

.overlay {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background-color: rgba(0, 0, 0, 0.5);
	z-index: 0;
}


@keyframes slide {
	0% {
		opacity: 0;
	}
	12.5% {
		opacity: 1;
	}
	25% {
		opacity: 1;
	}
	37.5% {
		opacity: 0;
	}
	100% {
		opacity: 0;
	}
}

.slider-container img:nth-child(1) {
	animation: slide 120s infinite;
}

.slider-container img:nth-child(2) {
	animation: slide 120s infinite 10s;
}

.slider-container img:nth-child(3) {
	animation: slide 120s infinite 20s;
}

.slider-container img:nth-child(4) {
	animation: slide 120s infinite 30s;
}
