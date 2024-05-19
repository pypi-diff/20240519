# Comparing `tmp/gradio_textlabeler-1.0.0.tar.gz` & `tmp/gradio_textlabeler-1.0.1.tar.gz`

## Comparing `gradio_textlabeler-1.0.0.tar` & `gradio_textlabeler-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/backend/gradio_textlabeler/__init__.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/backend/gradio_textlabeler/textlabeler.py
--rw-r--r--   0        0        0    15958 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/backend/gradio_textlabeler/textlabeler.pyi
--rw-r--r--   0        0        0    74475 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/backend/gradio_textlabeler/templates/component/index.js
--rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/backend/gradio_textlabeler/templates/component/style.css
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/backend/gradio_textlabeler/templates/example/index.js
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/backend/gradio_textlabeler/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/demo/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/demo/css.css
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/demo/requirements.txt
--rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/demo/space.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/frontend/Example.svelte
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/frontend/Index.svelte
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/frontend/Labeler.svelte
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/frontend/gradio.config.js
--rw-r--r--   0        0        0   150154 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/frontend/package-lock.json
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/frontend/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/.gitignore
--rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10130 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/backend/gradio_textlabeler/__init__.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/backend/gradio_textlabeler/textlabeler.py
+-rw-r--r--   0        0        0    15958 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/backend/gradio_textlabeler/textlabeler.pyi
+-rw-r--r--   0        0        0    74478 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/backend/gradio_textlabeler/templates/component/index.js
+-rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/backend/gradio_textlabeler/templates/component/style.css
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/backend/gradio_textlabeler/templates/example/index.js
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/backend/gradio_textlabeler/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/demo/__init__.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/demo/css.css
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/demo/requirements.txt
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/demo/space.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/frontend/Example.svelte
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/frontend/Index.svelte
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/frontend/Labeler.svelte
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/frontend/gradio.config.js
+-rw-r--r--   0        0        0   150154 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/frontend/package-lock.json
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/frontend/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/.gitignore
+-rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/README.md
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_textlabeler-1.0.1/PKG-INFO
```

### Comparing `gradio_textlabeler-1.0.0/backend/gradio_textlabeler/textlabeler.py` & `gradio_textlabeler-1.0.1/backend/gradio_textlabeler/textlabeler.py`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/backend/gradio_textlabeler/textlabeler.pyi` & `gradio_textlabeler-1.0.1/backend/gradio_textlabeler/textlabeler.pyi`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/backend/gradio_textlabeler/templates/component/index.js` & `gradio_textlabeler-1.0.1/backend/gradio_textlabeler/templates/component/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     get_all_dirty_from_scope: ct,
     get_slot_changes: dt,
     get_spread_update: mt,
     init: bt,
     insert: ht,
     safe_not_equal: gt,
     set_dynamic_element_data: ll,
-    set_style: D,
+    set_style: H,
     toggle_class: X,
     transition_in: jl,
     transition_out: Pl,
     update_slot_base: wt
 } = window.__gradio__svelte__internal;
 
 function kt(n) {
@@ -74,46 +74,46 @@
             ), X(
                 e,
                 "border_contrast",
                 /*border_mode*/
                 n[5] === "contrast"
             ), X(e, "hide-container", ! /*explicit_call*/
                 n[8] && ! /*container*/
-                n[9]), D(
+                n[9]), H(
                 e,
                 "height",
                 /*get_dimension*/
                 n[15](
                     /*height*/
                     n[0]
                 )
-            ), D(e, "width", typeof /*width*/ n[1] == "number" ? `calc(min(${/*width*/
+            ), H(e, "width", typeof /*width*/ n[1] == "number" ? `calc(min(${/*width*/
       n[1]}px, 100%))` : (
                 /*get_dimension*/
                 n[15](
                     /*width*/
                     n[1]
                 )
-            )), D(
+            )), H(
                 e,
                 "border-style",
                 /*variant*/
                 n[4]
-            ), D(
+            ), H(
                 e,
                 "overflow",
                 /*allow_overflow*/
                 n[11] ? "visible" : "hidden"
-            ), D(
+            ), H(
                 e,
                 "flex-grow",
                 /*scale*/
                 n[12]
-            ), D(e, "min-width", `calc(min(${/*min_width*/
-      n[13]}px, 100%))`), D(e, "border-width", "var(--block-border-width)");
+            ), H(e, "min-width", `calc(min(${/*min_width*/
+      n[13]}px, 100%))`), H(e, "border-width", "var(--block-border-width)");
         },
         m(s, _) {
             ht(s, e, _), f && f.m(e, null), t = !0;
         },
         p(s, _) {
             f && f.p && (!t || _ & /*$$scope*/
                     131072) && wt(
@@ -175,50 +175,50 @@
                     e,
                     "border_contrast",
                     /*border_mode*/
                     s[5] === "contrast"
                 ), X(e, "hide-container", ! /*explicit_call*/
                     s[8] && ! /*container*/
                     s[9]), _ & /*height*/
-                1 && D(
+                1 && H(
                     e,
                     "height",
                     /*get_dimension*/
                     s[15](
                         /*height*/
                         s[0]
                     )
                 ), _ & /*width*/
-                2 && D(e, "width", typeof /*width*/ s[1] == "number" ? `calc(min(${/*width*/
+                2 && H(e, "width", typeof /*width*/ s[1] == "number" ? `calc(min(${/*width*/
       s[1]}px, 100%))` : (
                     /*get_dimension*/
                     s[15](
                         /*width*/
                         s[1]
                     )
                 )), _ & /*variant*/
-                16 && D(
+                16 && H(
                     e,
                     "border-style",
                     /*variant*/
                     s[4]
                 ), _ & /*allow_overflow*/
-                2048 && D(
+                2048 && H(
                     e,
                     "overflow",
                     /*allow_overflow*/
                     s[11] ? "visible" : "hidden"
                 ), _ & /*scale*/
-                4096 && D(
+                4096 && H(
                     e,
                     "flex-grow",
                     /*scale*/
                     s[12]
                 ), _ & /*min_width*/
-                8192 && D(e, "min-width", `calc(min(${/*min_width*/
+                8192 && H(e, "min-width", `calc(min(${/*min_width*/
       s[13]}px, 100%))`);
         },
         i(s) {
             t || (jl(f, s), t = !0);
         },
         o(s) {
             Pl(f, s), t = !1;
@@ -287,15 +287,15 @@
         visible: C = !0
     } = e, {
         allow_overflow: S = !0
     } = e, {
         scale: b = null
     } = e, {
         min_width: h = 0
-    } = e, q = c === "fieldset" ? "fieldset" : "div";
+    } = e, L = c === "fieldset" ? "fieldset" : "div";
     const N = (v) => {
         if (v !== void 0) {
             if (typeof v == "number")
                 return v + "px";
             if (typeof v == "string")
                 return v;
         }
@@ -313,15 +313,15 @@
         d,
         m,
         w,
         C,
         S,
         b,
         h,
-        q,
+        L,
         N,
         c,
         i,
         t
     ];
 }
 class yt extends st {
@@ -343,44 +343,44 @@
             scale: 12,
             min_width: 13
         });
     }
 }
 const {
     SvelteComponent: Ct,
-    attr: qt,
-    create_slot: Lt,
+    attr: Lt,
+    create_slot: qt,
     detach: St,
     element: Ft,
     get_all_dirty_from_scope: Vt,
     get_slot_changes: Nt,
     init: zt,
     insert: Mt,
-    safe_not_equal: Dt,
-    transition_in: Ht,
+    safe_not_equal: Ht,
+    transition_in: Dt,
     transition_out: It,
     update_slot_base: Ot
 } = window.__gradio__svelte__internal;
 
 function Zt(n) {
     let e, l;
     const t = (
             /*#slots*/
             n[1].default
         ),
-        i = Lt(
+        i = qt(
             t,
             n,
             /*$$scope*/
             n[0],
             null
         );
     return {
         c() {
-            e = Ft("div"), i && i.c(), qt(e, "class", "svelte-1hnfib2");
+            e = Ft("div"), i && i.c(), Lt(e, "class", "svelte-1hnfib2");
         },
         m(f, o) {
             Mt(f, e, o), i && i.m(e, null), l = !0;
         },
         p(f, [o]) {
             i && i.p && (!l || o & /*$$scope*/
                 1) && Ot(
@@ -399,15 +399,15 @@
                     /*$$scope*/
                     f[0]
                 ),
                 null
             );
         },
         i(f) {
-            l || (Ht(i, f), l = !0);
+            l || (Dt(i, f), l = !0);
         },
         o(f) {
             It(i, f), l = !1;
         },
         d(f) {
             f && St(e), i && i.d(f);
         }
@@ -421,25 +421,25 @@
     } = e;
     return n.$$set = (f) => {
         "$$scope" in f && l(0, i = f.$$scope);
     }, [i, t];
 }
 class Pt extends Ct {
     constructor(e) {
-        super(), zt(this, e, jt, Zt, Dt, {});
+        super(), zt(this, e, jt, Zt, Ht, {});
     }
 }
 const {
     SvelteComponent: Bt,
     attr: tl,
     check_outros: Wt,
     create_component: At,
-    create_slot: Et,
-    destroy_component: Tt,
-    detach: Le,
+    create_slot: Tt,
+    destroy_component: Et,
+    detach: qe,
     element: Xt,
     empty: Yt,
     get_all_dirty_from_scope: Gt,
     get_slot_changes: Rt,
     group_outros: Jt,
     init: Kt,
     insert: Se,
@@ -483,15 +483,15 @@
         i(t) {
             l || (he(e.$$.fragment, t), l = !0);
         },
         o(t) {
             Fe(e.$$.fragment, t), l = !1;
         },
         d(t) {
-            Tt(e, t);
+            Et(e, t);
         }
     };
 }
 
 function tn(n) {
     let e;
     return {
@@ -509,26 +509,26 @@
                 2 && xt(
                     e,
                     /*info*/
                     l[1]
                 );
         },
         d(l) {
-            l && Le(e);
+            l && qe(e);
         }
     };
 }
 
 function nn(n) {
     let e, l, t, i;
     const f = (
             /*#slots*/
             n[2].default
         ),
-        o = Et(
+        o = Tt(
             f,
             n,
             /*$$scope*/
             n[3],
             null
         );
     let a = (
@@ -587,15 +587,15 @@
         i(s) {
             i || (he(o, s), he(a), i = !0);
         },
         o(s) {
             Fe(o, s), Fe(a), i = !1;
         },
         d(s) {
-            s && (Le(e), Le(l), Le(t)), o && o.d(s), a && a.d(s);
+            s && (qe(e), qe(l), qe(t)), o && o.d(s), a && a.d(s);
         }
     };
 }
 
 function fn(n, e, l) {
     let {
         $$slots: t = {},
@@ -930,16 +930,16 @@
         });
     }
 }
 const {
     SvelteComponent: Cn,
     append: je,
     attr: Z,
-    detach: qn,
-    init: Ln,
+    detach: Ln,
+    init: qn,
     insert: Sn,
     noop: Pe,
     safe_not_equal: Fn,
     set_style: Y,
     svg_element: ye
 } = window.__gradio__svelte__internal;
 
@@ -952,21 +952,21 @@
         m(f, o) {
             Sn(f, e, o), je(e, l), je(l, t), je(e, i);
         },
         p: Pe,
         i: Pe,
         o: Pe,
         d(f) {
-            f && qn(e);
+            f && Ln(e);
         }
     };
 }
 class Nn extends Cn {
     constructor(e) {
-        super(), Ln(this, e, null, Vn, Fn, {});
+        super(), qn(this, e, null, Vn, Fn, {});
     }
 }
 const zn = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
@@ -1325,40 +1325,40 @@
 function Ve() {}
 
 function Mn(n, e) {
     return n != n ? e == e : n !== e || n && typeof n == "object" || typeof n == "function";
 }
 const Al = typeof window < "u";
 let ol = Al ? () => window.performance.now() : () => Date.now(),
-    El = Al ? (n) => requestAnimationFrame(n) : Ve;
+    Tl = Al ? (n) => requestAnimationFrame(n) : Ve;
 const ce = /* @__PURE__ */ new Set();
 
-function Tl(n) {
+function El(n) {
     ce.forEach((e) => {
         e.c(n) || (ce.delete(e), e.f());
-    }), ce.size !== 0 && El(Tl);
+    }), ce.size !== 0 && Tl(El);
 }
 
-function Dn(n) {
+function Hn(n) {
     let e;
-    return ce.size === 0 && El(Tl), {
+    return ce.size === 0 && Tl(El), {
         promise: new Promise((l) => {
             ce.add(e = {
                 c: n,
                 f: l
             });
         }),
         abort() {
             ce.delete(e);
         }
     };
 }
 const _e = [];
 
-function Hn(n, e = Ve) {
+function Dn(n, e = Ve) {
     let l;
     const t = /* @__PURE__ */ new Set();
 
     function i(a) {
         if (Mn(n, a) && (n = a, l)) {
             const s = !_e.length;
             for (const _ of t)
@@ -1388,66 +1388,66 @@
     };
 }
 
 function sl(n) {
     return Object.prototype.toString.call(n) === "[object Date]";
 }
 
-function Ee(n, e, l, t) {
+function Te(n, e, l, t) {
     if (typeof l == "number" || sl(l)) {
         const i = t - l,
             f = (l - e) / (n.dt || 1 / 60),
             o = n.opts.stiffness * i,
             a = n.opts.damping * f,
             s = (o - a) * n.inv_mass,
             _ = (f + s) * n.dt;
         return Math.abs(_) < n.opts.precision && Math.abs(i) < n.opts.precision ? t : (n.settled = !1, sl(l) ? new Date(l.getTime() + _) : l + _);
     } else {
         if (Array.isArray(l))
             return l.map(
-                (i, f) => Ee(n, e[f], l[f], t[f])
+                (i, f) => Te(n, e[f], l[f], t[f])
             );
         if (typeof l == "object") {
             const i = {};
             for (const f in l)
-                i[f] = Ee(n, e[f], l[f], t[f]);
+                i[f] = Te(n, e[f], l[f], t[f]);
             return i;
         } else
             throw new Error(`Cannot spring ${typeof l} values`);
     }
 }
 
 function al(n, e = {}) {
-    const l = Hn(n),
+    const l = Dn(n),
         {
             stiffness: t = 0.15,
             damping: i = 0.8,
             precision: f = 0.01
         } = e;
     let o, a, s, _ = n,
         r = n,
         u = 1,
         c = 0,
         d = !1;
 
     function m(C, S = {}) {
         r = C;
         const b = s = {};
-        return n == null || S.hard || w.stiffness >= 1 && w.damping >= 1 ? (d = !0, o = ol(), _ = C, l.set(n = r), Promise.resolve()) : (S.soft && (c = 1 / ((S.soft === !0 ? 0.5 : +S.soft) * 60), u = 0), a || (o = ol(), d = !1, a = Dn((h) => {
+        return n == null || S.hard || w.stiffness >= 1 && w.damping >= 1 ? (d = !0, o = ol(), _ = C, l.set(n = r), Promise.resolve()) : (S.soft && (c = 1 / ((S.soft === !0 ? 0.5 : +S.soft) * 60), u = 0), a || (o = ol(), d = !1, a = Hn((h) => {
             if (d)
                 return d = !1, a = null, !1;
             u = Math.min(u + c, 1);
-            const q = {
+            const L = {
                     inv_mass: u,
                     opts: w,
                     settled: !0,
                     dt: (h - o) * 60 / 1e3
                 },
-                N = Ee(q, _, n, r);
-            return o = h, _ = n, l.set(n = N), q.settled && (a = null), !q.settled;
+                N = Te(L, _, n, r);
+            return o = h, _ = n, l.set(n = N), L.settled && (a = null), !L.settled;
         })), new Promise((h) => {
             a.promise.then(() => {
                 b === s && h();
             });
         }));
     }
     const w = {
@@ -1459,15 +1459,15 @@
         precision: f
     };
     return w;
 }
 const {
     SvelteComponent: In,
     append: j,
-    attr: L,
+    attr: q,
     component_subscribe: _l,
     detach: On,
     element: Zn,
     init: jn,
     insert: Pn,
     noop: rl,
     safe_not_equal: Bn,
@@ -1478,19 +1478,19 @@
     onMount: Wn
 } = window.__gradio__svelte__internal;
 
 function An(n) {
     let e, l, t, i, f, o, a, s, _, r, u, c;
     return {
         c() {
-            e = Zn("div"), l = P("svg"), t = P("g"), i = P("path"), f = P("path"), o = P("path"), a = P("path"), s = P("g"), _ = P("path"), r = P("path"), u = P("path"), c = P("path"), L(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), L(i, "fill", "#FF7C00"), L(i, "fill-opacity", "0.4"), L(i, "class", "svelte-43sxxs"), L(f, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), L(f, "fill", "#FF7C00"), L(f, "class", "svelte-43sxxs"), L(o, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), L(o, "fill", "#FF7C00"), L(o, "fill-opacity", "0.4"), L(o, "class", "svelte-43sxxs"), L(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), L(a, "fill", "#FF7C00"), L(a, "class", "svelte-43sxxs"), Ce(t, "transform", "translate(" + /*$top*/
+            e = Zn("div"), l = P("svg"), t = P("g"), i = P("path"), f = P("path"), o = P("path"), a = P("path"), s = P("g"), _ = P("path"), r = P("path"), u = P("path"), c = P("path"), q(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(f, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(f, "fill", "#FF7C00"), q(f, "class", "svelte-43sxxs"), q(o, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(o, "fill", "#FF7C00"), q(o, "fill-opacity", "0.4"), q(o, "class", "svelte-43sxxs"), q(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(a, "fill", "#FF7C00"), q(a, "class", "svelte-43sxxs"), Ce(t, "transform", "translate(" + /*$top*/
                 n[1][0] + "px, " + /*$top*/
-                n[1][1] + "px)"), L(_, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), L(_, "fill", "#FF7C00"), L(_, "fill-opacity", "0.4"), L(_, "class", "svelte-43sxxs"), L(r, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), L(r, "fill", "#FF7C00"), L(r, "class", "svelte-43sxxs"), L(u, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), L(u, "fill", "#FF7C00"), L(u, "fill-opacity", "0.4"), L(u, "class", "svelte-43sxxs"), L(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), L(c, "fill", "#FF7C00"), L(c, "class", "svelte-43sxxs"), Ce(s, "transform", "translate(" + /*$bottom*/
+                n[1][1] + "px)"), q(_, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(_, "fill", "#FF7C00"), q(_, "fill-opacity", "0.4"), q(_, "class", "svelte-43sxxs"), q(r, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(r, "fill", "#FF7C00"), q(r, "class", "svelte-43sxxs"), q(u, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(u, "fill", "#FF7C00"), q(u, "fill-opacity", "0.4"), q(u, "class", "svelte-43sxxs"), q(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(c, "fill", "#FF7C00"), q(c, "class", "svelte-43sxxs"), Ce(s, "transform", "translate(" + /*$bottom*/
                 n[2][0] + "px, " + /*$bottom*/
-                n[2][1] + "px)"), L(l, "viewBox", "-1200 -1200 3000 3000"), L(l, "fill", "none"), L(l, "xmlns", "http://www.w3.org/2000/svg"), L(l, "class", "svelte-43sxxs"), L(e, "class", "svelte-43sxxs"), ul(
+                n[2][1] + "px)"), q(l, "viewBox", "-1200 -1200 3000 3000"), q(l, "fill", "none"), q(l, "xmlns", "http://www.w3.org/2000/svg"), q(l, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), ul(
                 e,
                 "margin",
                 /*margin*/
                 n[0]
             );
         },
         m(d, m) {
@@ -1515,24 +1515,24 @@
         o: rl,
         d(d) {
             d && On(e);
         }
     };
 }
 
-function En(n, e, l) {
+function Tn(n, e, l) {
     let t, i;
     var f = this && this.__awaiter || function(d, m, w, C) {
         function S(b) {
             return b instanceof w ? b : new w(function(h) {
                 h(b);
             });
         }
         return new(w || (w = Promise))(function(b, h) {
-            function q(g) {
+            function L(g) {
                 try {
                     v(C.next(g));
                 } catch (J) {
                     h(J);
                 }
             }
 
@@ -1541,15 +1541,15 @@
                     v(C.throw(g));
                 } catch (J) {
                     h(J);
                 }
             }
 
             function v(g) {
-                g.done ? b(g.value) : S(g.value).then(q, N);
+                g.done ? b(g.value) : S(g.value).then(L, N);
             }
             v((C = C.apply(d, m || [])).next());
         });
     };
     let {
         margin: o = !0
     } = e;
@@ -1576,27 +1576,27 @@
             yield Promise.all([a.set([125, 0]), s.set([-125, 0])]), u();
         });
     }
     return Wn(() => (c(), () => _ = !0)), n.$$set = (d) => {
         "margin" in d && l(0, o = d.margin);
     }, [o, t, i, a, s];
 }
-class Tn extends In {
+class En extends In {
     constructor(e) {
-        super(), jn(this, e, En, An, Bn, {
+        super(), jn(this, e, Tn, An, Bn, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: Xn,
     append: te,
     attr: A,
     binding_callbacks: cl,
-    check_outros: Te,
+    check_outros: Ee,
     create_component: Xl,
     create_slot: Yl,
     destroy_component: Gl,
     destroy_each: Rl,
     detach: p,
     element: G,
     empty: de,
@@ -1609,15 +1609,15 @@
     mount_component: Ql,
     noop: Ye,
     safe_not_equal: Gn,
     set_data: O,
     set_style: U,
     space: I,
     text: F,
-    toggle_class: H,
+    toggle_class: D,
     transition_in: W,
     transition_out: R,
     update_slot_base: Ul
 } = window.__gradio__svelte__internal, {
     tick: Rn
 } = window.__gradio__svelte__internal, {
     onDestroy: Jn
@@ -1715,15 +1715,15 @@
     let e, l, t, i, f, o, a, s, _, r = (
         /*variant*/
         n[8] === "default" && /*show_eta_bar*/
         n[18] && /*show_progress*/
         n[6] === "full" && gl(n)
     );
 
-    function u(h, q) {
+    function u(h, L) {
         if (
             /*progress*/
             h[7]
         )
             return ti;
         if (
             /*queue_position*/
@@ -1743,68 +1743,68 @@
         m = (
             /*timer*/
             n[5] && vl(n)
         );
     const w = [oi, fi],
         C = [];
 
-    function S(h, q) {
+    function S(h, L) {
         return (
             /*last_progress_level*/
             h[15] != null ? 0 : (
                 /*show_progress*/
                 h[6] === "full" ? 1 : -1
             )
         );
     }
     ~(f = S(n)) && (o = C[f] = w[f](n));
     let b = ! /*timer*/
         n[5] && Fl(n);
     return {
         c() {
-            r && r.c(), e = I(), l = G("div"), d && d.c(), t = I(), m && m.c(), i = I(), o && o.c(), a = I(), b && b.c(), s = de(), A(l, "class", "progress-text svelte-vopvsi"), H(
+            r && r.c(), e = I(), l = G("div"), d && d.c(), t = I(), m && m.c(), i = I(), o && o.c(), a = I(), b && b.c(), s = de(), A(l, "class", "progress-text svelte-vopvsi"), D(
                 l,
                 "meta-text-center",
                 /*variant*/
                 n[8] === "center"
-            ), H(
+            ), D(
                 l,
                 "meta-text",
                 /*variant*/
                 n[8] === "default"
             );
         },
-        m(h, q) {
-            r && r.m(h, q), y(h, e, q), y(h, l, q), d && d.m(l, null), te(l, t), m && m.m(l, null), y(h, i, q), ~f && C[f].m(h, q), y(h, a, q), b && b.m(h, q), y(h, s, q), _ = !0;
+        m(h, L) {
+            r && r.m(h, L), y(h, e, L), y(h, l, L), d && d.m(l, null), te(l, t), m && m.m(l, null), y(h, i, L), ~f && C[f].m(h, L), y(h, a, L), b && b.m(h, L), y(h, s, L), _ = !0;
         },
-        p(h, q) {
+        p(h, L) {
             /*variant*/
             h[8] === "default" && /*show_eta_bar*/
                 h[18] && /*show_progress*/
-                h[6] === "full" ? r ? r.p(h, q) : (r = gl(h), r.c(), r.m(e.parentNode, e)) : r && (r.d(1), r = null), c === (c = u(h)) && d ? d.p(h, q) : (d && d.d(1), d = c && c(h), d && (d.c(), d.m(l, t))), /*timer*/
-                h[5] ? m ? m.p(h, q) : (m = vl(h), m.c(), m.m(l, null)) : m && (m.d(1), m = null), (!_ || q[0] & /*variant*/
-                    256) && H(
+                h[6] === "full" ? r ? r.p(h, L) : (r = gl(h), r.c(), r.m(e.parentNode, e)) : r && (r.d(1), r = null), c === (c = u(h)) && d ? d.p(h, L) : (d && d.d(1), d = c && c(h), d && (d.c(), d.m(l, t))), /*timer*/
+                h[5] ? m ? m.p(h, L) : (m = vl(h), m.c(), m.m(l, null)) : m && (m.d(1), m = null), (!_ || L[0] & /*variant*/
+                    256) && D(
                     l,
                     "meta-text-center",
                     /*variant*/
                     h[8] === "center"
-                ), (!_ || q[0] & /*variant*/
-                    256) && H(
+                ), (!_ || L[0] & /*variant*/
+                    256) && D(
                     l,
                     "meta-text",
                     /*variant*/
                     h[8] === "default"
                 );
             let N = f;
-            f = S(h), f === N ? ~f && C[f].p(h, q) : (o && (Xe(), R(C[N], 1, 1, () => {
+            f = S(h), f === N ? ~f && C[f].p(h, L) : (o && (Xe(), R(C[N], 1, 1, () => {
                     C[N] = null;
-                }), Te()), ~f ? (o = C[f], o ? o.p(h, q) : (o = C[f] = w[f](h), o.c()), W(o, 1), o.m(a.parentNode, a)) : o = null), /*timer*/
+                }), Ee()), ~f ? (o = C[f], o ? o.p(h, L) : (o = C[f] = w[f](h), o.c()), W(o, 1), o.m(a.parentNode, a)) : o = null), /*timer*/
                 h[5] ? b && (Xe(), R(b, 1, 1, () => {
                     b = null;
-                }), Te()) : b ? (b.p(h, q), q[0] & /*timer*/
+                }), Ee()) : b ? (b.p(h, L), L[0] & /*timer*/
                     32 && W(b, 1)) : (b = Fl(h), b.c(), W(b, 1), b.m(s.parentNode, s));
         },
         i(h) {
             _ || (W(o), W(b), _ = !0);
         },
         o(h) {
             R(o), R(b), _ = !1;
@@ -2074,15 +2074,15 @@
             f && (p(e), p(t), p(i));
         }
     };
 }
 
 function fi(n) {
     let e, l;
-    return e = new Tn({
+    return e = new En({
         props: {
             margin: (
                 /*variant*/
                 n[8] === "default"
             )
         }
     }), {
@@ -2192,19 +2192,19 @@
         a = (
             /*p*/
             n[41].desc != null && /*progress_level*/
             n[14] && /*progress_level*/
             n[14][
                 /*i*/
                 n[43]
-            ] != null && ql()
+            ] != null && Ll()
         ),
         s = (
             /*progress_level*/
-            n[14] != null && Ll(n)
+            n[14] != null && ql(n)
         );
     return {
         c() {
             f && f.c(), e = I(), o && o.c(), l = I(), a && a.c(), t = I(), s && s.c(), i = de();
         },
         m(_, r) {
             f && f.m(_, r), y(_, e, r), o && o.m(_, r), y(_, l, r), a && a.m(_, r), y(_, t, r), s && s.m(_, r), y(_, i, r);
@@ -2213,16 +2213,16 @@
             /*p*/
             _[41].desc != null ? o ? o.p(_, r) : (o = Cl(_), o.c(), o.m(l.parentNode, l)) : o && (o.d(1), o = null), /*p*/
                 _[41].desc != null && /*progress_level*/
                 _[14] && /*progress_level*/
                 _[14][
                     /*i*/
                     _[43]
-                ] != null ? a || (a = ql(), a.c(), a.m(t.parentNode, t)) : a && (a.d(1), a = null), /*progress_level*/
-                _[14] != null ? s ? s.p(_, r) : (s = Ll(_), s.c(), s.m(i.parentNode, i)) : s && (s.d(1), s = null);
+                ] != null ? a || (a = Ll(), a.c(), a.m(t.parentNode, t)) : a && (a.d(1), a = null), /*progress_level*/
+                _[14] != null ? s ? s.p(_, r) : (s = ql(_), s.c(), s.m(i.parentNode, i)) : s && (s.d(1), s = null);
         },
         d(_) {
             _ && (p(e), p(l), p(t), p(i)), f && f.d(_), o && o.d(_), a && a.d(_), s && s.d(_);
         }
     };
 }
 
@@ -2261,30 +2261,30 @@
         },
         d(t) {
             t && p(l);
         }
     };
 }
 
-function ql(n) {
+function Ll(n) {
     let e;
     return {
         c() {
             e = F("-");
         },
         m(l, t) {
             y(l, e, t);
         },
         d(l) {
             l && p(e);
         }
     };
 }
 
-function Ll(n) {
+function ql(n) {
     let e = (100 * /*progress_level*/
             (n[14][
                 /*i*/
                 n[43]
             ] || 0)).toFixed(1) + "",
         l, t;
     return {
@@ -2415,32 +2415,32 @@
             )
         );
     }
     return ~(l = s(n)) && (t = a[l] = o[l](n)), {
         c() {
             e = G("div"), t && t.c(), A(e, "class", i = "wrap " + /*variant*/
                 n[8] + " " + /*show_progress*/
-                n[6] + " svelte-vopvsi"), H(e, "hide", ! /*status*/
+                n[6] + " svelte-vopvsi"), D(e, "hide", ! /*status*/
                 n[4] || /*status*/
                 n[4] === "complete" || /*show_progress*/
-                n[6] === "hidden"), H(
+                n[6] === "hidden"), D(
                 e,
                 "translucent",
                 /*variant*/
                 n[8] === "center" && /*status*/
                 (n[4] === "pending" || /*status*/
                     n[4] === "error") || /*translucent*/
                 n[11] || /*show_progress*/
                 n[6] === "minimal"
-            ), H(
+            ), D(
                 e,
                 "generating",
                 /*status*/
                 n[4] === "generating"
-            ), H(
+            ), D(
                 e,
                 "border",
                 /*border*/
                 n[12]
             ), U(
                 e,
                 "position",
@@ -2456,39 +2456,39 @@
         m(_, r) {
             y(_, e, r), ~l && a[l].m(e, null), n[33](e), f = !0;
         },
         p(_, r) {
             let u = l;
             l = s(_), l === u ? ~l && a[l].p(_, r) : (t && (Xe(), R(a[u], 1, 1, () => {
                     a[u] = null;
-                }), Te()), ~l ? (t = a[l], t ? t.p(_, r) : (t = a[l] = o[l](_), t.c()), W(t, 1), t.m(e, null)) : t = null), (!f || r[0] & /*variant, show_progress*/
+                }), Ee()), ~l ? (t = a[l], t ? t.p(_, r) : (t = a[l] = o[l](_), t.c()), W(t, 1), t.m(e, null)) : t = null), (!f || r[0] & /*variant, show_progress*/
                     320 && i !== (i = "wrap " + /*variant*/
                         _[8] + " " + /*show_progress*/
                         _[6] + " svelte-vopvsi")) && A(e, "class", i), (!f || r[0] & /*variant, show_progress, status, show_progress*/
-                    336) && H(e, "hide", ! /*status*/
+                    336) && D(e, "hide", ! /*status*/
                     _[4] || /*status*/
                     _[4] === "complete" || /*show_progress*/
                     _[6] === "hidden"), (!f || r[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
-                    2384) && H(
+                    2384) && D(
                     e,
                     "translucent",
                     /*variant*/
                     _[8] === "center" && /*status*/
                     (_[4] === "pending" || /*status*/
                         _[4] === "error") || /*translucent*/
                     _[11] || /*show_progress*/
                     _[6] === "minimal"
                 ), (!f || r[0] & /*variant, show_progress, status*/
-                    336) && H(
+                    336) && D(
                     e,
                     "generating",
                     /*status*/
                     _[4] === "generating"
                 ), (!f || r[0] & /*variant, show_progress, border*/
-                    4416) && H(
+                    4416) && D(
                     e,
                     "border",
                     /*border*/
                     _[12]
                 ), r[0] & /*absolute*/
                 1024 && U(
                     e,
@@ -2539,34 +2539,34 @@
 
         function _(r) {
             r.done ? f(r.value) : i(r.value).then(a, s);
         }
         _((t = t.apply(n, e || [])).next());
     });
 };
-let qe = [],
+let Le = [],
     Be = !1;
 
 function ri(n) {
     return _i(this, arguments, void 0, function*(e, l = !0) {
         if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && l !== !0)) {
-            if (qe.push(e), !Be)
+            if (Le.push(e), !Be)
                 Be = !0;
             else
                 return;
             yield Rn(), requestAnimationFrame(() => {
                 let t = [0, 0];
-                for (let i = 0; i < qe.length; i++) {
-                    const o = qe[i].getBoundingClientRect();
+                for (let i = 0; i < Le.length; i++) {
+                    const o = Le[i].getBoundingClientRect();
                     (i === 0 || o.top + window.scrollY <= t[0]) && (t[0] = o.top + window.scrollY, t[1] = i);
                 }
                 window.scrollTo({
                     top: t[0] - 20,
                     behavior: "smooth"
-                }), Be = !1, qe = [];
+                }), Be = !1, Le = [];
             });
         }
     });
 }
 
 function ui(n, e, l) {
     let t, {
@@ -2598,15 +2598,15 @@
     } = e, {
         variant: S = "default"
     } = e, {
         loading_text: b = "Loading..."
     } = e, {
         absolute: h = !0
     } = e, {
-        translucent: q = !1
+        translucent: L = !1
     } = e, {
         border: N = !1
     } = e, {
         autoscroll: v
     } = e, g, J = !1, ge = 0, x = 0, fe = null, oe = null, Ue = 0, $ = null, me, Q = null, xe = !0;
     const $l = () => {
         l(0, s = l(27, fe = l(19, we = null))), l(25, ge = performance.now()), l(26, x = 0), J = !0, $e();
@@ -2637,15 +2637,15 @@
 
     function tt(k) {
         cl[k ? "unshift" : "push"](() => {
             g = k, l(13, g);
         });
     }
     return n.$$set = (k) => {
-        "i18n" in k && l(1, a = k.i18n), "eta" in k && l(0, s = k.eta), "queue_position" in k && l(2, _ = k.queue_position), "queue_size" in k && l(3, r = k.queue_size), "status" in k && l(4, u = k.status), "scroll_to_output" in k && l(22, c = k.scroll_to_output), "timer" in k && l(5, d = k.timer), "show_progress" in k && l(6, m = k.show_progress), "message" in k && l(23, w = k.message), "progress" in k && l(7, C = k.progress), "variant" in k && l(8, S = k.variant), "loading_text" in k && l(9, b = k.loading_text), "absolute" in k && l(10, h = k.absolute), "translucent" in k && l(11, q = k.translucent), "border" in k && l(12, N = k.border), "autoscroll" in k && l(24, v = k.autoscroll), "$$scope" in k && l(29, f = k.$$scope);
+        "i18n" in k && l(1, a = k.i18n), "eta" in k && l(0, s = k.eta), "queue_position" in k && l(2, _ = k.queue_position), "queue_size" in k && l(3, r = k.queue_size), "status" in k && l(4, u = k.status), "scroll_to_output" in k && l(22, c = k.scroll_to_output), "timer" in k && l(5, d = k.timer), "show_progress" in k && l(6, m = k.show_progress), "message" in k && l(23, w = k.message), "progress" in k && l(7, C = k.progress), "variant" in k && l(8, S = k.variant), "loading_text" in k && l(9, b = k.loading_text), "absolute" in k && l(10, h = k.absolute), "translucent" in k && l(11, L = k.translucent), "border" in k && l(12, N = k.border), "autoscroll" in k && l(24, v = k.autoscroll), "$$scope" in k && l(29, f = k.$$scope);
     }, n.$$.update = () => {
         n.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
             436207617 && (s === null && l(0, s = fe), s != null && fe !== s && (l(28, oe = (performance.now() - ge) / 1e3 + s), l(19, we = oe.toFixed(1)), l(27, fe = s))), n.$$.dirty[0] & /*eta_from_start, timer_diff*/
             335544320 && l(17, Ue = oe === null || oe <= 0 || !x ? null : Math.min(x / oe, 1)), n.$$.dirty[0] & /*progress*/
             128 && C != null && l(18, xe = !1), n.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
             114816 && (C != null ? l(14, $ = C.map((k) => {
                 if (k.index != null && k.length != null)
@@ -2665,15 +2665,15 @@
         u,
         d,
         m,
         C,
         S,
         b,
         h,
-        q,
+        L,
         N,
         g,
         $,
         me,
         Q,
         Ue,
         xe,
@@ -2725,20 +2725,20 @@
     }
 }
 const {
     SvelteComponent: di,
     append: V,
     attr: B,
     destroy_each: xl,
-    detach: E,
+    detach: T,
     element: M,
     empty: Qe,
     ensure_array_like: ze,
     init: mi,
-    insert: T,
+    insert: E,
     listen: bi,
     noop: Vl,
     safe_not_equal: hi,
     select_option: Nl,
     set_data: ne,
     set_input_value: Ge,
     set_style: Re,
@@ -2774,15 +2774,15 @@
                 n[7]
             ), _ = Me(), r = M("tbody");
             for (let d = 0; d < c.length; d += 1)
                 c[d].c();
             B(i, "class", "svelte-1i7yt9n"), B(a, "class", "svelte-1i7yt9n"), B(t, "class", "svelte-1i7yt9n"), B(l, "class", "svelte-1i7yt9n"), B(r, "class", "svelte-1i7yt9n"), B(e, "width", "100%"), Re(e, "text-align", "left"), B(e, "class", "svelte-1i7yt9n");
         },
         m(d, m) {
-            T(d, e, m), V(e, l), V(l, t), V(t, i), V(i, f), V(t, o), V(t, a), V(a, s), V(e, _), V(e, r);
+            E(d, e, m), V(e, l), V(l, t), V(t, i), V(i, f), V(t, o), V(t, a), V(a, s), V(e, _), V(e, r);
             for (let w = 0; w < c.length; w += 1)
                 c[w] && c[w].m(r, null);
         },
         p(d, m) {
             if (m & /*textColumnHeader*/
                 32 && ne(
                     f,
@@ -2806,15 +2806,15 @@
                 }
                 for (; w < c.length; w += 1)
                     c[w].d(1);
                 c.length = u.length;
             }
         },
         d(d) {
-            d && E(e), xl(c, d);
+            d && T(e), xl(c, d);
         }
     };
 }
 
 function wi(n) {
     let e;
 
@@ -2827,21 +2827,21 @@
     let t = l(n),
         i = t(n);
     return {
         c() {
             i.c(), e = Qe();
         },
         m(f, o) {
-            i.m(f, o), T(f, e, o);
+            i.m(f, o), E(f, e, o);
         },
         p(f, o) {
             t !== (t = l(f)) && (i.d(1), i = t(f), i && (i.c(), i.m(e.parentNode, e)));
         },
         d(f) {
-            f && E(e), i.d(f);
+            f && T(e), i.d(f);
         }
     };
 }
 
 function ki(n) {
     let e = (
             /*valueItem*/
@@ -2849,61 +2849,61 @@
         ),
         l;
     return {
         c() {
             l = ie(e);
         },
         m(t, i) {
-            T(t, l, i);
+            E(t, l, i);
         },
         p(t, i) {
             i & /*value*/
                 1 && e !== (e = /*valueItem*/
                     t[11].label + "") && ne(l, e);
         },
         d(t) {
-            t && E(l);
+            t && T(l);
         }
     };
 }
 
 function vi(n) {
     let e;
     return {
         c() {
             e = ie(
                 /*unlabelledValueDisplay*/
                 n[4]
             );
         },
         m(l, t) {
-            T(l, e, t);
+            E(l, e, t);
         },
         p(l, t) {
             t & /*unlabelledValueDisplay*/
                 16 && ne(
                     e,
                     /*unlabelledValueDisplay*/
                     l[4]
                 );
         },
         d(l) {
-            l && E(e);
+            l && T(e);
         }
     };
 }
 
 function pi(n) {
     let e, l, t, i, f, o, a = ze(
             /*labels*/
             n[3]
         ),
         s = [];
     for (let r = 0; r < a.length; r += 1)
-        s[r] = Hl(Ml(n, a, r));
+        s[r] = Dl(Ml(n, a, r));
 
     function _(...r) {
         return (
             /*change_handler*/
             n[10](
                 /*i*/
                 n[13],
@@ -2918,15 +2918,15 @@
                 n[4]
             );
             for (let r = 0; r < s.length; r += 1)
                 s[r].c();
             l.__value = "!!unlabeled", Ge(l, l.__value), B(e, "class", "svelte-1i7yt9n");
         },
         m(r, u) {
-            T(r, e, u), V(e, l), V(l, t);
+            E(r, e, u), V(e, l), V(l, t);
             for (let c = 0; c < s.length; c += 1)
                 s[c] && s[c].m(e, null);
             Nl(
                 e,
                 /*valueItem*/
                 n[11].label === null ? "!!unlabeled" : (
                     /*valueItem*/
@@ -2945,15 +2945,15 @@
                 a = ze(
                     /*labels*/
                     n[3]
                 );
                 let c;
                 for (c = 0; c < a.length; c += 1) {
                     const d = Ml(n, a, c);
-                    s[c] ? s[c].p(d, u) : (s[c] = Hl(d), s[c].c(), s[c].m(e, null));
+                    s[c] ? s[c].p(d, u) : (s[c] = Dl(d), s[c].c(), s[c].m(e, null));
                 }
                 for (; c < s.length; c += 1)
                     s[c].d(1);
                 s.length = a.length;
             }
             u & /*value, labels*/
                 9 && i !== (i = /*valueItem*/
@@ -2966,76 +2966,76 @@
                     n[11].label === null ? "!!unlabeled" : (
                         /*valueItem*/
                         n[11].label
                     )
                 );
         },
         d(r) {
-            r && E(e), xl(s, r), f = !1, o();
+            r && T(e), xl(s, r), f = !1, o();
         }
     };
 }
 
-function Dl(n) {
+function Hl(n) {
     let e, l = (
             /*label*/
             n[14] + ""
         ),
         t, i;
     return {
         c() {
             e = M("option"), t = ie(l), e.__value = i = /*label*/
                 n[14], Ge(e, e.__value);
         },
         m(f, o) {
-            T(f, e, o), V(e, t);
+            E(f, e, o), V(e, t);
         },
         p(f, o) {
             o & /*labels*/
                 8 && l !== (l = /*label*/
                     f[14] + "") && ne(t, l), o & /*labels*/
                 8 && i !== (i = /*label*/
                     f[14]) && (e.__value = i, Ge(e, e.__value));
         },
         d(f) {
-            f && E(e);
+            f && T(e);
         }
     };
 }
 
-function Hl(n) {
+function Dl(n) {
     let e = ! /*onlySelectLabelOnce*/
         n[1] || ! /*selectedLabels*/
         n[8].has(
             /*label*/
             n[14]
         ) || /*label*/
         n[14] === /*valueItem*/
         n[11].label,
-        l, t = e && Dl(n);
+        l, t = e && Hl(n);
     return {
         c() {
             t && t.c(), l = Qe();
         },
         m(i, f) {
-            t && t.m(i, f), T(i, l, f);
+            t && t.m(i, f), E(i, l, f);
         },
         p(i, f) {
             f & /*onlySelectLabelOnce, selectedLabels, labels, value*/
                 267 && (e = ! /*onlySelectLabelOnce*/
                     i[1] || ! /*selectedLabels*/
                     i[8].has(
                         /*label*/
                         i[14]
                     ) || /*label*/
                     i[14] === /*valueItem*/
-                    i[11].label), e ? t ? t.p(i, f) : (t = Dl(i), t.c(), t.m(l.parentNode, l)) : t && (t.d(1), t = null);
+                    i[11].label), e ? t ? t.p(i, f) : (t = Hl(i), t.c(), t.m(l.parentNode, l)) : t && (t.d(1), t = null);
         },
         d(i) {
-            i && E(l), t && t.d(i);
+            i && T(l), t && t.d(i);
         }
     };
 }
 
 function Il(n) {
     let e, l, t = (
             /*valueItem*/
@@ -3060,64 +3060,64 @@
                 l,
                 "width",
                 /*textColumnWidth*/
                 n[6]
             ), B(l, "class", "svelte-1i7yt9n"), B(o, "class", "svelte-1i7yt9n"), B(e, "class", "svelte-1i7yt9n");
         },
         m(u, c) {
-            T(u, e, c), V(e, l), V(l, i), V(e, f), V(e, o), r.m(o, null), V(e, a);
+            E(u, e, c), V(e, l), V(l, i), V(e, f), V(e, o), r.m(o, null), V(e, a);
         },
         p(u, c) {
             c & /*value*/
                 1 && t !== (t = /*valueItem*/
                     u[11].text + "") && ne(i, t), c & /*textColumnWidth*/
                 64 && Re(
                     l,
                     "width",
                     /*textColumnWidth*/
                     u[6]
                 ), _ === (_ = s(u)) && r ? r.p(u, c) : (r.d(1), r = _(u), r && (r.c(), r.m(o, null)));
         },
         d(u) {
-            u && E(e), r.d();
+            u && T(e), r.d();
         }
     };
 }
 
 function yi(n) {
     let e;
     return {
         c() {
             e = M("p"), e.textContent = "No labeling data to show";
         },
         m(l, t) {
-            T(l, e, t);
+            E(l, e, t);
         },
         d(l) {
-            l && E(e);
+            l && T(e);
         }
     };
 }
 
 function Ci(n) {
     let e;
     return {
         c() {
             e = M("p"), e.textContent = "No data to label";
         },
         m(l, t) {
-            T(l, e, t);
+            E(l, e, t);
         },
         d(l) {
-            l && E(e);
+            l && T(e);
         }
     };
 }
 
-function qi(n) {
+function Li(n) {
     let e;
 
     function l(f, o) {
         return (
             /*value*/
             f[0].length === 0 ? wi : gi
         );
@@ -3125,28 +3125,28 @@
     let t = l(n),
         i = t(n);
     return {
         c() {
             i.c(), e = Qe();
         },
         m(f, o) {
-            i.m(f, o), T(f, e, o);
+            i.m(f, o), E(f, e, o);
         },
         p(f, [o]) {
             t === (t = l(f)) && i ? i.p(f, o) : (i.d(1), i = t(f), i && (i.c(), i.m(e.parentNode, e)));
         },
         i: Vl,
         o: Vl,
         d(f) {
-            f && E(e), i.d(f);
+            f && T(e), i.d(f);
         }
     };
 }
 
-function Li(n, e, l) {
+function qi(n, e, l) {
     let {
         onlySelectLabelOnce: t = !1
     } = e, {
         value: i
     } = e, {
         interactive: f = !1
     } = e, {
@@ -3191,15 +3191,15 @@
         u,
         c,
         d
     ];
 }
 class Si extends di {
     constructor(e) {
-        super(), mi(this, e, Li, qi, hi, {
+        super(), mi(this, e, qi, Li, hi, {
             onlySelectLabelOnce: 1,
             value: 0,
             interactive: 2,
             labels: 3,
             unlabelledValueDisplay: 4,
             textColumnHeader: 5,
             textColumnWidth: 6,
@@ -3209,19 +3209,19 @@
 }
 const {
     SvelteComponent: Fi,
     add_flush_callback: Vi,
     assign: Ni,
     bind: zi,
     binding_callbacks: Mi,
-    check_outros: Di,
-    create_component: De,
-    destroy_component: He,
+    check_outros: Hi,
+    create_component: He,
+    destroy_component: De,
     detach: Je,
-    get_spread_object: Hi,
+    get_spread_object: Di,
     get_spread_update: Ii,
     group_outros: Oi,
     init: Zi,
     insert: Ke,
     mount_component: Ie,
     safe_not_equal: ji,
     set_data: Pi,
@@ -3254,15 +3254,15 @@
         props: i
     }), e.$on(
         "clear_status",
         /*clear_status_handler*/
         n[17]
     ), {
         c() {
-            De(e.$$.fragment);
+            He(e.$$.fragment);
         },
         m(f, o) {
             Ie(e, f, o), l = !0;
         },
         p(f, o) {
             const a = o & /*gradio, loading_status*/
                 49152 ? Ii(t, [
@@ -3277,29 +3277,29 @@
                     32768 && {
                         i18n: (
                             /*gradio*/
                             f[15].i18n
                         )
                     },
                     o & /*loading_status*/
-                    16384 && Hi(
+                    16384 && Di(
                         /*loading_status*/
                         f[14]
                     )
                 ]) : {};
             e.$set(a);
         },
         i(f) {
             l || (le(e.$$.fragment, f), l = !0);
         },
         o(f) {
             ue(e.$$.fragment, f), l = !1;
         },
         d(f) {
-            He(e, f);
+            De(e, f);
         }
     };
 }
 
 function Wi(n) {
     let e;
     return {
@@ -3381,25 +3381,25 @@
     return (
         /*value*/
         n[0] !== void 0 && (_.value = /*value*/
             n[0]), i = new Si({
             props: _
         }), Mi.push(() => zi(i, "value", s)), {
             c() {
-                a && a.c(), e = Ol(), De(l.$$.fragment), t = Ol(), De(i.$$.fragment);
+                a && a.c(), e = Ol(), He(l.$$.fragment), t = Ol(), He(i.$$.fragment);
             },
             m(r, u) {
                 a && a.m(r, u), Ke(r, e, u), Ie(l, r, u), Ke(r, t, u), Ie(i, r, u), o = !0;
             },
             p(r, u) {
                 /*loading_status*/
                 r[14] ? a ? (a.p(r, u), u & /*loading_status*/
                     16384 && le(a, 1)) : (a = Zl(r), a.c(), le(a, 1), a.m(e.parentNode, e)) : a && (Oi(), ue(a, 1, 1, () => {
                     a = null;
-                }), Di());
+                }), Hi());
                 const c = {};
                 u & /*show_label*/
                     2048 && (c.show_label = /*show_label*/
                         r[11]), u & /*$$scope, label*/
                     1048578 && (c.$$scope = {
                         dirty: u,
                         ctx: r
@@ -3426,21 +3426,21 @@
             i(r) {
                 o || (le(a), le(l.$$.fragment, r), le(i.$$.fragment, r), o = !0);
             },
             o(r) {
                 ue(a), ue(l.$$.fragment, r), ue(i.$$.fragment, r), o = !1;
             },
             d(r) {
-                r && (Je(e), Je(t)), a && a.d(r), He(l, r), He(i, r);
+                r && (Je(e), Je(t)), a && a.d(r), De(l, r), De(i, r);
             }
         }
     );
 }
 
-function Ei(n) {
+function Ti(n) {
     let e, l;
     return e = new yt({
         props: {
             visible: (
                 /*visible*/
                 n[4]
             ),
@@ -3448,15 +3448,15 @@
                 /*elem_id*/
                 n[2]
             ),
             elem_classes: (
                 /*elem_classes*/
                 n[3]
             ),
-            padding: Ti,
+            padding: Ei,
             allow_overflow: !1,
             scale: (
                 /*scale*/
                 n[12]
             ),
             min_width: (
                 /*min_width*/
@@ -3467,15 +3467,15 @@
             },
             $$scope: {
                 ctx: n
             }
         }
     }), {
         c() {
-            De(e.$$.fragment);
+            He(e.$$.fragment);
         },
         m(t, i) {
             Ie(e, t, i), l = !0;
         },
         p(t, [i]) {
             const f = {};
             i & /*visible*/
@@ -3497,23 +3497,23 @@
         i(t) {
             l || (le(e.$$.fragment, t), l = !0);
         },
         o(t) {
             ue(e.$$.fragment, t), l = !1;
         },
         d(t) {
-            He(e, t);
+            De(e, t);
         }
     };
 }
-const Ti = !0;
+const Ei = !0;
 
 function Xi(n, e, l) {
     let {
-        label: t = "Dropdown"
+        label: t = "TextLabeler"
     } = e, {
         elem_id: i = ""
     } = e, {
         elem_classes: f = []
     } = e, {
         visible: o = !0
     } = e, {
@@ -3540,27 +3540,27 @@
         loading_status: S
     } = e, {
         gradio: b
     } = e, {
         interactive: h
     } = e;
 
-    function q() {
+    function L() {
         b.dispatch("change");
     }
     const N = () => b.dispatch("clear_status", S);
 
     function v(g) {
         a = g, l(0, a);
     }
     return n.$$set = (g) => {
         "label" in g && l(1, t = g.label), "elem_id" in g && l(2, i = g.elem_id), "elem_classes" in g && l(3, f = g.elem_classes), "visible" in g && l(4, o = g.visible), "value" in g && l(0, a = g.value), "label_choices" in g && l(5, s = g.label_choices), "text_column_width" in g && l(6, _ = g.text_column_width), "allow_duplicate_labels" in g && l(7, r = g.allow_duplicate_labels), "unlabelled_value_display" in g && l(8, u = g.unlabelled_value_display), "text_column_header" in g && l(9, c = g.text_column_header), "label_column_header" in g && l(10, d = g.label_column_header), "show_label" in g && l(11, m = g.show_label), "scale" in g && l(12, w = g.scale), "min_width" in g && l(13, C = g.min_width), "loading_status" in g && l(14, S = g.loading_status), "gradio" in g && l(15, b = g.gradio), "interactive" in g && l(16, h = g.interactive);
     }, n.$$.update = () => {
         n.$$.dirty & /*value*/
-            1 && q();
+            1 && L();
     }, [
         a,
         t,
         i,
         f,
         o,
         s,
@@ -3577,15 +3577,15 @@
         h,
         N,
         v
     ];
 }
 class Yi extends Fi {
     constructor(e) {
-        super(), Zi(this, e, Xi, Ei, ji, {
+        super(), Zi(this, e, Xi, Ti, ji, {
             label: 1,
             elem_id: 2,
             elem_classes: 3,
             visible: 4,
             value: 0,
             label_choices: 5,
             text_column_width: 6,
```

### Comparing `gradio_textlabeler-1.0.0/backend/gradio_textlabeler/templates/component/style.css` & `gradio_textlabeler-1.0.1/backend/gradio_textlabeler/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/backend/gradio_textlabeler/templates/example/index.js` & `gradio_textlabeler-1.0.1/backend/gradio_textlabeler/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/demo/app.py` & `gradio_textlabeler-1.0.1/demo/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from gradio_textlabeler.textlabeler import TextLabelerData
 import gradio as gr
 from gradio_textlabeler import TextLabeler
 
 
-example = TextLabeler().example_value()
-
-demo = gr.Interface(
-    lambda x: x,
-    TextLabeler(
+with gr.Blocks() as demo:
+    gr.Markdown("abel the tweets as positive, negative, or neutral and click on Submit Labels")
+    inp = TextLabeler(
+        label="Label these tweets",
+        info="Label the tweets as positive, negative, or neutral.",
         label_choices=["Positive", "Negative", "Neutral"],
         value=[
             {"text": "I am extremely mad", "label": "Negative"},
             {
                 "text": "This product is the next best thing since sliced bread",
                 "label": "Positive",
             },
@@ -21,14 +21,16 @@
             {"text": "I'm not sure what to think", "label": None},
         ],
         allow_duplicate_labels=True,
         unlabelled_value_display="No Label",
         text_column_width="60%",
         text_column_header="Tweet",
         label_column_header="Sentiment",
-    ),  
-    TextLabeler(),  
-)
+    )   
+    btn = gr.Button("Submit Labels")
+    out = TextLabeler(label="Label output example")
+   
+    btn.click(fn=lambda x:x, inputs=inp, outputs=out)
 
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_textlabeler-1.0.0/demo/css.css` & `gradio_textlabeler-1.0.1/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/demo/space.py` & `gradio_textlabeler-1.0.1/demo/space.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `gradio_textlabeler`
 
 <div style="display: flex; gap: 7px;">
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%201.0.0%20-%20orange"> <a href="https://github.com/amithkk/gradio_textlabeler/issues" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/Issues-white?logo=github&logoColor=black"></a> 
+<a href="https://pypi.org/project/gradio_textlabeler/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_textlabeler"></a> <a href="https://github.com/amithkk/gradio_textlabeler/issues" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/Issues-white?logo=github&logoColor=black"></a> 
 </div>
 
 A Gradio custom component to help you label text snippets inline
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
@@ -39,19 +39,19 @@
 
 ```python
 from gradio_textlabeler.textlabeler import TextLabelerData
 import gradio as gr
 from gradio_textlabeler import TextLabeler
 
 
-example = TextLabeler().example_value()
-
-demo = gr.Interface(
-    lambda x: x,
-    TextLabeler(
+with gr.Blocks() as demo:
+    gr.Markdown("abel the tweets as positive, negative, or neutral and click on Submit Labels")
+    inp = TextLabeler(
+        label="Label these tweets",
+        info="Label the tweets as positive, negative, or neutral.",
         label_choices=["Positive", "Negative", "Neutral"],
         value=[
             {"text": "I am extremely mad", "label": "Negative"},
             {
                 "text": "This product is the next best thing since sliced bread",
                 "label": "Positive",
             },
@@ -61,17 +61,19 @@
             {"text": "I'm not sure what to think", "label": None},
         ],
         allow_duplicate_labels=True,
         unlabelled_value_display="No Label",
         text_column_width="60%",
         text_column_header="Tweet",
         label_column_header="Sentiment",
-    ),  
-    TextLabeler(),  
-)
+    )   
+    btn = gr.Button("Submit Labels")
+    out = TextLabeler(label="Label output example")
+   
+    btn.click(fn=lambda x:x, inputs=inp, outputs=out)
 
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
 """, elem_classes=["md-custom"], header_links=True)
```

### Comparing `gradio_textlabeler-1.0.0/frontend/Index.svelte` & `gradio_textlabeler-1.0.1/frontend/Index.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <script lang="ts">
 	import type { Gradio } from "@gradio/utils";
 	import { Block, BlockTitle } from "@gradio/atoms";
 	import { StatusTracker } from "@gradio/statustracker";
 	import type { LoadingStatus } from "@gradio/statustracker";
 	import Labeler from "./Labeler.svelte";
 
-	export let label = "Dropdown";
+	export let label = "TextLabeler";
 	export let elem_id = "";
 	export let elem_classes: string[] = [];
 	export let visible = true;
 	export let value: { text: string; label: string }[];
 	export let label_choices: string[];
 	export let text_column_width: string;
 	export let allow_duplicate_labels: boolean;
```

### Comparing `gradio_textlabeler-1.0.0/frontend/Labeler.svelte` & `gradio_textlabeler-1.0.1/frontend/Labeler.svelte`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/frontend/package-lock.json` & `gradio_textlabeler-1.0.1/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/frontend/package.json` & `gradio_textlabeler-1.0.1/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_textlabeler-1.0.0/README.md` & `gradio_textlabeler-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
-tags: [gradio-custom-component, SimpleDropdown]
+tags: [gradio-custom-component, TextLabeler]
 title: gradio_textlabeler
-short_description: 
+short_description: A Gradio custom component to help you label text snippets
 colorFrom: blue
 colorTo: yellow
 sdk: gradio
 pinned: false
 app_file: space.py
 ---
 
 # `gradio_textlabeler`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%201.0.0%20-%20orange"> <a href="https://github.com/amithkk/gradio_textlabeler/issues" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/Issues-white?logo=github&logoColor=black"></a> 
+<a href="https://pypi.org/project/gradio_textlabeler/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_textlabeler"></a> <a href="https://github.com/amithkk/gradio_textlabeler/issues" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/Issues-white?logo=github&logoColor=black"></a> 
 
 A Gradio custom component to help you label text snippets inline
 
 ## Installation
 
 ```bash
 pip install gradio_textlabeler
@@ -24,19 +24,19 @@
 
 ```python
 from gradio_textlabeler.textlabeler import TextLabelerData
 import gradio as gr
 from gradio_textlabeler import TextLabeler
 
 
-example = TextLabeler().example_value()
-
-demo = gr.Interface(
-    lambda x: x,
-    TextLabeler(
+with gr.Blocks() as demo:
+    gr.Markdown("abel the tweets as positive, negative, or neutral and click on Submit Labels")
+    inp = TextLabeler(
+        label="Label these tweets",
+        info="Label the tweets as positive, negative, or neutral.",
         label_choices=["Positive", "Negative", "Neutral"],
         value=[
             {"text": "I am extremely mad", "label": "Negative"},
             {
                 "text": "This product is the next best thing since sliced bread",
                 "label": "Positive",
             },
@@ -46,17 +46,19 @@
             {"text": "I'm not sure what to think", "label": None},
         ],
         allow_duplicate_labels=True,
         unlabelled_value_display="No Label",
         text_column_width="60%",
         text_column_header="Tweet",
         label_column_header="Sentiment",
-    ),  
-    TextLabeler(),  
-)
+    )   
+    btn = gr.Button("Submit Labels")
+    out = TextLabeler(label="Label output example")
+   
+    btn.click(fn=lambda x:x, inputs=inp, outputs=out)
 
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
```

### Comparing `gradio_textlabeler-1.0.0/pyproject.toml` & `gradio_textlabeler-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_textlabeler"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Gradio custom component to help you label text snippets inline"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Amith K K", email = "amithkumaran@gmail.com" }]
-keywords = ["gradio-custom-component", "gradio-template-SimpleDropdown"]
+keywords = ["gradio-custom-component"]
 # Add dependencies here
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'Operating System :: OS Independent',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
```

### Comparing `gradio_textlabeler-1.0.0/PKG-INFO` & `gradio_textlabeler-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: gradio_textlabeler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Gradio custom component to help you label text snippets inline
 Project-URL: repository, https://github.com/amithkk/gradio_textlabeler
 Author-email: Amith K K <amithkumaran@gmail.com>
 License-Expression: Apache-2.0
-Keywords: gradio-custom-component,gradio-template-SimpleDropdown
+Keywords: gradio-custom-component
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,26 +21,26 @@
 Requires-Dist: gradio<5.0,>=4.0
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 ---
-tags: [gradio-custom-component, SimpleDropdown]
+tags: [gradio-custom-component, TextLabeler]
 title: gradio_textlabeler
-short_description: 
+short_description: A Gradio custom component to help you label text snippets
 colorFrom: blue
 colorTo: yellow
 sdk: gradio
 pinned: false
 app_file: space.py
 ---
 
 # `gradio_textlabeler`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%201.0.0%20-%20orange"> <a href="https://github.com/amithkk/gradio_textlabeler/issues" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/Issues-white?logo=github&logoColor=black"></a> 
+<a href="https://pypi.org/project/gradio_textlabeler/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_textlabeler"></a> <a href="https://github.com/amithkk/gradio_textlabeler/issues" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/Issues-white?logo=github&logoColor=black"></a> 
 
 A Gradio custom component to help you label text snippets inline
 
 ## Installation
 
 ```bash
 pip install gradio_textlabeler
@@ -50,19 +50,19 @@
 
 ```python
 from gradio_textlabeler.textlabeler import TextLabelerData
 import gradio as gr
 from gradio_textlabeler import TextLabeler
 
 
-example = TextLabeler().example_value()
-
-demo = gr.Interface(
-    lambda x: x,
-    TextLabeler(
+with gr.Blocks() as demo:
+    gr.Markdown("abel the tweets as positive, negative, or neutral and click on Submit Labels")
+    inp = TextLabeler(
+        label="Label these tweets",
+        info="Label the tweets as positive, negative, or neutral.",
         label_choices=["Positive", "Negative", "Neutral"],
         value=[
             {"text": "I am extremely mad", "label": "Negative"},
             {
                 "text": "This product is the next best thing since sliced bread",
                 "label": "Positive",
             },
@@ -72,17 +72,19 @@
             {"text": "I'm not sure what to think", "label": None},
         ],
         allow_duplicate_labels=True,
         unlabelled_value_display="No Label",
         text_column_width="60%",
         text_column_header="Tweet",
         label_column_header="Sentiment",
-    ),  
-    TextLabeler(),  
-)
+    )   
+    btn = gr.Button("Submit Labels")
+    out = TextLabeler(label="Label output example")
+   
+    btn.click(fn=lambda x:x, inputs=inp, outputs=out)
 
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
```

