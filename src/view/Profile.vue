<template>
  <b-container>
    <b-row class="text-center">
      <b-col cols="12">
        <img :src="$auth.user.picture"/>
      </b-col>
      <b-col cols="12">
        <h2>{{ $auth.user.name }}</h2>
        <p>{{ $auth.user.email }}</p>
      </b-col>
      <b-col cols="12">
        <div>
          <p>{{ $auth.user.given_name }}</p>
          <p>{{ $auth.user.family_name }}</p>
          <p>{{ $auth.user.nickname }}</p>
          <p>{{ $auth.user.locale }}</p>
          <p>{{ $auth.user.updated_at }}</p>
          <p>{{ $auth.user.email_verified }}</p>
          <p>{{ $auth.user.sub }}</p>
        </div>
      </b-col>
    </b-row>
  </b-container>
</template>