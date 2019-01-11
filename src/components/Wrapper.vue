<script>
export default {
  data() {
    return {
      mutate: () => {
        this.val = this.val + 1;
      },
      val: 0
    };
  },
  render() {
    return this.$scopedSlots.default({
      mutate: this.mutate,
      val: this.val
    });
  }
};
</script>
