<template>
  <div class="brand-overlay">
    <img src="/images/logo.png" class="brand-logo" />
    <div class="brand-footer">
      <span class="brand-footer-left">Think Equity. Think Motilal Oswal.</span>
      <span class="brand-footer-right">www.motilaloswalgroup.com</span>
    </div>
  </div>
</template>

<style scoped>
.brand-overlay {
  position: absolute;
  inset: 0;
  pointer-events: none;
  z-index: 100;
}

.brand-logo {
  position: absolute;
  top: 12px;
  right: 16px;
  height: 52px;
  width: auto;
}

.brand-footer {
  position: absolute;
  bottom: 8px;
  left: 20px;
  right: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 0.6rem;
  color: #303192;
  opacity: 0.7;
}
</style>
