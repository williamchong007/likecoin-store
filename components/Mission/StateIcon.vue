<template>
  <div :class="['mission-state-icon', layout, state]">
    <loading-indicator
      v-if="state === 'pending'"
      :layout="layout"
    />
    <mission-clock
      v-if="state === 'cooldown'"
    />
  </div>
</template>


<script>
import LoadingIndicator from './LoadingIndicator';
import MissionClock from './Clock';

export default {
  name: 'mission-state-icon',
  components: {
    LoadingIndicator,
    MissionClock,
  },
  props: {
    layout: {
      type: String,
      validator(value) {
        return ['small', 'large', 'fluid'].indexOf(value) !== -1;
      },
      default: 'fluid',
    },
    state: {
      type: String,
      default: undefined,
    },
  },
};
</script>


<style lang="scss" scoped>
@import "~assets/variables";

@mixin large-mission-state-icon {
  width: 52px;
  height: 52px;

  padding: 10px;

  border-radius: 50%;
  background-color: white;

  &::before {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;

    margin: 3px;

    content: " ";

    border-radius: 50%;
  }

  &.active,
  &.completed,
  &.pending,
  &.upcoming,
  &.cooldown {
    box-shadow: 0 1px 5px 1px rgba(0, 0, 0, 0.3);
  }

  &.active,
  &.pending,
  &.cooldown {
    background-image: linear-gradient(215deg, #D2F0F0, #F0E6B4);

    &::before {
      background-color: white;
    }
  }

  &.active {
    &::after {
      mask: url('~assets/mission/misc/active.svg');

      background-color: $like-green;
    }
  }

  &.completed,
  &.claimed {
    &::after {
      mask: url('~assets/mission/misc/completed.svg');

      background-color: $like-white;
    }
  }

  &.completed {
    &::before {
      background-color: $like-green-2;
    }
  }

  &.claimed {
    background-color: $like-green;
  }

  &.pending,
  &.cooldown {
    background-image: linear-gradient(215deg, #D2F0F0, #F0E6B4);

    &::after {
      height: 0;
    }
  }

  &.upcoming {
    border: solid 2px #e6e6e6;
  }
}

@mixin small-mission-state-icon {
  width: 32px;
  height: 32px;

  &.active {
    &::after {
      mask: url('~assets/mission/misc/active-small.svg');

      background-color: $like-green;
    }
  }

  &.completed,
  &.claimed {
    &::after {
      mask: url('~assets/mission/misc/completed-small.svg');
    }
  }

  &.completed::after {
    background-color: $like-white;
  }
  &.claimed::after {
    background-color: #9b9b9b;
  }
}

.mission-state-icon {
  position: relative;

  &::after {
    position: relative;

    display: block;

    width: 100%;
    height: 100%;

    content: " ";

    background-repeat: no-repeat;
    background-position: center;
    background-size: 32px 32px;
  }

  &.small {
    @include small-mission-state-icon();
  }

  &.large {
    @include large-mission-state-icon();
  }

  &.fluid {
    @media (min-width: 600px + 1px) {
      @include large-mission-state-icon();
    }

    @media (max-width: 600px) {
      @include small-mission-state-icon();
    }
  }

  &.upcoming {
    &::after {
      mask: url('~assets/mission/misc/upcoming.svg');

      background-color: #9b9b9b;
    }
  }
}
</style>
